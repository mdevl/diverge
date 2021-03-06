= diverge

Diverge is a very simple class for calculating the Kullback–Leibler divergence or Jensen–Shannon divergence of two datasets. Example usage is as follows:

    1.9.3p194 :001 > require "diverge"
    => true 
    1.9.3p194 :002 > Diverge.new([0.25, 0.5, 0.25], [0.5, 0.3, 0.2]).kl # Kullback-Leibler
    => 0.1379119045715615 
    1.9.3p194 :003 > Diverge.new([0.25, 0.5, 0.25], [0.5, 0.3, 0.2]).kl(:reverse)
    => 0.14869719288733346 
    1.9.3p194 :004 > Diverge.new([0.5, 0.3, 0.2], [0.25, 0.5, 0.25]).kl
    => 0.14869719288733346 
    1.9.3p194 :005 > Diverge.new([0.25, 0.5, 0.25], [0.5, 0.3, 0.2]).js # Jensen-Shannon
    => 0.14330454872944748 
    1.9.3p194 :006 > Diverge.new([0.5, 0.3, 0.2], [0.25, 0.5, 0.25]).js
    => 0.14330454872944748
    1.9.3p194 :006 > Diverge.new([0.5, 0.3, 0.2], [0.25, 0.5, 0.25]).corr # Pearson correlation
    => -0.18898223650461368

http://rubygems.org/gems/diverge

== Contributing to diverge
 
* Check out the latest master to make sure the feature hasn't been implemented or the bug hasn't been fixed yet.
* Check out the issue tracker to make sure someone already hasn't requested it and/or contributed it.
* Fork the project.
* Start a feature/bugfix branch.
* Commit and push until you are happy with your contribution.
* Make sure to add tests for it. This is important so I don't break it in a future version unintentionally.
* Please try not to mess with the Rakefile, version, or history. If you want to have your own version, or is otherwise necessary, that is fine, but please isolate to its own commit so I can cherry-pick around it.

== Copyright

Copyright (c) 2012 Evan Senter. See LICENSE.txt for
further details.

