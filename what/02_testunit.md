!SLIDE bullets

Test::Unit
==========

* The original Ruby xUnit framework
* In Ruby 1.8 stdlib
* <http://ruby-doc.org/stdlib/libdoc/test/unit/rdoc/>

!SLIDE

Test::Unit
============

    @@@ Ruby
    class TestAddition < Test::Unit::TestCase
      def test_addition
        assert_equal(4, 2 + 2)
      end
    end
