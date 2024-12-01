# Add `Parameters#expect` to safely filter and require params

 ```ruby
 # URLに`?person=hacked`というパラメータが指定されていた場合

 # Before
 params.require(:person).permit(:name, :age, pets: [:name])
 # => NoMethodErrorをraiseして500エラー

 # After
 params.expect(person: [ :name, :age, pets: [[:name]] ])
 # => ActionController::ParameterMissingをraiseして400エラー
```
