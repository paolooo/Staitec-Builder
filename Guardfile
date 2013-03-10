# A sample Guardfile
# More info at https://github.com/guard/guard#readme

interactor :off

guard 'haml', :output => 'public', :input => 'app/views' do
  watch %r{^app/views/.+(\.html\.haml)}
end

guard 'coffeescript', :input => 'app/coffee', :output => 'public/javascripts'

guard 'compass' do
  watch %r{^app/sass/(.*)\.s[ac]ss}
end
