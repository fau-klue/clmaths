require 'html-proofer'

desc "Build and test website"

task :test do

  # Will output the _site directory
  sh "bundle exec jekyll build"

  # Options for html-proofer
  options = {
    :disable_external => true,
    :url_swap => {'/clmaths' => ''},
    :verbose => true
  }

  HTMLProofer.check_directory("./_site", options).run
end
