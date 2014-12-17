task :server do
  sh "rackup"
end

desc "Generate a graphic"
task :client do
  require 'rest_client'
  RestClient.post 'http://localhost:9292/graphs/sample', :value => rand(99)
end

desc "View generated graphic"
task :view do
  sh "open http://localhosst:9292/graphs/sample"
end
