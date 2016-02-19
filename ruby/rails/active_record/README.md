# ActiveRecord

TIL's about the ActiveRecord framework

### Scratch

* Row level locking: `user.lock!` and `user.with_lock {}`
    * [ActiveRecord::Locking::Pessimistic](http://api.rubyonrails.org/classes/ActiveRecord/Locking/Pessimistic.html)
