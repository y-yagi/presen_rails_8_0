# [Add `Parameters#expect` to safely filter and require params (#51674)](https://github.com/rails/rails/commit/e1d58cfd05ae1cc0bfc1006b7ce973a7730831df)

 ```ruby
 # URLに`?person=hacked`というパラメータが指定されていた場合

 # Before
 params.require(:person).permit(:name, :age, pets: [:name])
 # => NoMethodErrorをraiseして500エラー

 # After
 params.expect(person: [ :name, :age, pets: [[:name]] ])
 # => ActionController::ParameterMissingraiseして400エラー
```
