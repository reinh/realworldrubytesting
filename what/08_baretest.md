!SLIDE smbullets

Baretest
========

* BDD style framework
* Straightforward and terse assertions
* Formatters, including XML and TAP
* "Suites" with dependency declarations
* Helpers for raising, floats, collections, etc
* Interactive mode
* <http://github.com/apeiros/baretest>

!SLIDE small

Baretest
========

    @@@ Ruby
    BareTest.suite do
      suite "Dependencies", :requires => ['foo', 'bar'] do
        assert "Will be skipped" do
          failure "Nothing to see here"
        end
      end
    end
