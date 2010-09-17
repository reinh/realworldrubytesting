!SLIDE bullets

RSpec
=====

* The de facto standard BDD framework
* Used by many popular Ruby libraries
* <http://rspec.info>

!SLIDE

RSpec
=====

    @@@ Ruby
      describe Bowling, "#score" do
        it "returns 0 for all gutter game" do
          bowling = Bowling.new
          20.times { bowling.hit(0) }
          bowling.score.should == 0
        end
      end
