!SLIDE bullets

Micronaut
=========

* Light-weight BDD framework
* API compatible with RSpec
* With metadata, like "Focused examples"
* Or custom metadata
* <http://github.com/spicycode/micronaut>

!SLIDE small

Micronaut
=========

    @@@ Ruby
    describe Micronaut do
      describe "#configure" do
        focused "should yield the current configuration" do
          Micronaut.configure do |config|
            config.should == Micronaut.configuration
          end
        end

        it "should be callable without a block" do
          Micronaut.configure
        end
      end
    end
