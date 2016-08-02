# Useful Enumerable methods (can be called on Hash objects and Array objects):

* `all?`
* `any?`
* `count`
* `each_slice`
* `each_with_index`
* `each_with_object`
* `find`
* `find_all`
* `find_index`
* `include?`
* `map`
* `max`
* `min`
* `none?`
* `reduce`
* `reject`
* `select`
* `sort`
* `sort_by`
* `to_a`
* `to_h`
* `zip`

# Useful Enumerator methods
* with_index
* with_object

Note: Enumerator methods can be chained to any Enumerable method that returns
an Enumerator object. For example: Enumerable method `select`, [if it is not
passed a block, returns an Enumerator
object](http://ruby-doc.org/core-2.3.1/Enumerable.html#method-i-select), so we
can chain `with_index` onto `select`, like this:

```ruby
["hello", "goodbye", "hello again"].select.with_index do |str, index|
  index.even? && str.length > 5
end
# => ["hello again"]
```

# Useful Array methods

* `+`
* `-`
* `<<`
* `==`
* `[]`
* `[]=`
* `any?`
* `compact`
* `compact!`
* `count`
* `delete`
* `delete_at`
* `delete_if`
* `dig`
* `each`
* `empty?`
* `find_index`
* `first`
* `flatten`
* `flatten!`
* `include?`
* `index`
* `join`
* `length`
* `map`
* `map!`
* `permutation`
* `pop`
* `push`
* `reject`
* `reject!`
* `reverse`
* `reverse!`
* `rotate`
* `rotate!`
* `sample`
* `select`
* `select!`
* `shift`
* `shuffle`
* `shuffle!`
* `slice`
* `slice!`
* `sort`
* `sort!`
* `sort_by!`
* `transpose`
* `uniq`
* `uniq!`
* `unshift`
* `zip`

# Useful Hash methods:

* `::[]`
* `::new`
* `[]`
* `[]=`
* `delete`
* `delete_if`
* `dig`
* `each`
* `each_key`
* `each_pair`
* `each_value`
* `fetch`
* `has_key?`
* `has_value?`
* `include?`
* `keep_if`
* `key?`
* `keys`
* `member?`
* `merge`
* `merge!`
