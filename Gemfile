source "http://rubygems.org"
gemspec

gem 'rake'

rails = ENV['RAILS'] || '3-2-stable'

arel = ENV['AREL'] || '3-0-stable'

arel_opts = case arel
when /\// # A path
  {:path => arel}
when /^v/ # A tagged version
  {:git => 'git://github.com/rails/arel.git', :tag => arel}
else
  {:git => 'git://github.com/rails/arel.git', :branch => arel}
end

gem 'arel', arel_opts

# case rails
# when /\// # A path
#   gem 'activesupport', :path => "#{rails}/activesupport"
#   gem 'activemodel', :path => "#{rails}/activemodel"
#   gem 'activerecord', :path => "#{rails}/activerecord"
# when /^v/ # A tagged version
#   git 'git://github.com/rails/rails.git', :tag => rails do
gem 'activesupport', '4.0.0.beta1'
gem 'activemodel', '4.0.0.beta1'
gem 'activerecord', '4.0.0.beta1'
#   end
# else
#   git 'git://github.com/rails/rails.git', :branch => rails do
#     gem 'activesupport'
#     gem 'activemodel'
#     gem 'activerecord'
#   end
# end
