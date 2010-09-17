!SLIDE bullets

Minitest
========

* Replaces Test::Unit in 1.9
* mini/spec BDD framework
* mini/mock mock object framework
* <http://github.com/seattlerb/minitest>

!SLIDE smaller

Minitest — Test::Unit Style
==========================

    @@@ Ruby
    class TestMeme < MiniTest::Unit::TestCase
      def setup
        @meme = Meme.new
      end

      def test_that_kitty_can_eat
        assert_equal "OHAI!", @meme.i_can_has_cheezburger?
      end

      def test_that_it_doesnt_not_blend
        refute_match /^no/i, @meme.does_it_blend?
      end
    end

!SLIDE smaller

Minitest — Spec Style
====================

    @@@ Ruby
    describe Meme do
      before do
        @meme = Meme.new
      end

      describe "when asked about cheeseburgers" do
        it "should respond positively" do
          @meme.i_can_has_cheezburger?.must_equal "OHAI!"
        end
      end

      describe "when asked about blending possibilities" do
        it "won't say no" do
          @meme.does_it_blend?.wont_match /^no/i
        end
      end
    end

