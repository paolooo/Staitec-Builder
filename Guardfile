# A sample Guardfile
# More info at https://github.com/guard/guard#readme

interactor :off

guard 'haml', :input => 'app/views' do
  watch %r{^app/views/.+(\.html\.haml)}
end

guard 'coffeescript', :input => 'app/coffee', :output => 'javascripts'

#guard 'compass' do
#  watch %r{^app/sass/(.*)\.s[ac]ss}
#end

#guard 'livereload', :host => '127.0.0.1', :port => '35729' do
guard 'livereload' do
  #watch(%r{app/views/.+\.(\.html\.haml)$})
  watch(%r{.+\.(html)$})
  watch(%r{stylesheets/.+\.(css)})
  watch(%r{javascripts/.+\.(js)})
  # Rails Assets Pipeline
  #watch(%r{(app|vendor)(/assets/\w+/(.+\.(css|js|html))).*}) { |m| "/assets/#{m[3]}" }
end

# Add files and commands to this file, like the example:
#   watch(%r{file/path}) { `command(s)` }
#
#guard 'shell' do
#  #watch(/(.*).txt/) {|m| `tail #{m[0]}` }
#  watch(%r{(stylesheets/.+\.css)}) { |m| `cp -R #{m[0]} ../stylesheets` }
#  watch(%r{(javascripts/.+\.js)}) { |m| `cp -R #{m[0]} ../javascripts` }
#  watch(%r{(images/.+\.(png|jpg|gif))}) { |m| `cp -R #{m[0]} ../images` }
#  watch(%r{(.+\.html)}) { |m| `cp -R #{m[0]} ../` }
#end
