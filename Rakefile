require 'html-proofer'

desc "build and test website"
task :test do
  sh "bundle exec jekyll build"

  options = {
    :disable_external => true,
    :url_swap => {'/clmaths' => ''},
    :verbose => true
  }

  HTMLProofer.check_directory("./_site", options).run
end
