!SLIDE bullets

Riot
====

* No setup or teardown
* `setup` defines a "topic"
* Like Rspec's `subject`
* <http://github.com/thumblemonks/riot>

!SLIDE

Riot
====

    @@@ Ruby
    context "An Array" do
      setup { Array.new }
      asserts("is empty") { topic.empty? }
    end
 
