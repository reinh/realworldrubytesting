!SLIDE bullets

Bacon
=====

* (Very) lightweight RSpec clone
* Less than 350 LoC 
* That's not a lot of code
* <http://github.com/chneukirchen/bacon>

!SLIDE

Bacon
=====

    @@@ Ruby
    describe 'A new array' do
      before do
        @ary = Array.new
      end

      it 'should be empty' do
        @ary.should.be.empty
        @ary.should.not.include 1
      end
    end
