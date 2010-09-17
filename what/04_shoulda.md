!SLIDE smbullets

Shoulda
=======

* Bolt-on BDD framework for Test::Unit
* Adds `context` and `should`
* Many helpful Matchers and assertions
* Built-in Rails testing idioms
* Matchers also RSpec compatible
* <http://github.com/thoughtbot/shoulda>

!SLIDE

Shoulda
=======

    @@@ Ruby
    class PostTest < Test::Unit::TestCase
      should belong_to(:user)
      should have_many(:tags).through(:taggings)

      should validate_uniqueness_of(:title)
      should validate_presence_of(:title)
      should validate_numericality_of(:user_id)
    end
