require 'kata_chapter'

task :default => :build

desc 'Build Katas from sources'
task :build do
  FileUtils.rm_rf('build')
  Dir.glob('src/*/sections.yaml').each do |chapter|
    puts "building #{chapter}"
    KataChapter.new(chapter).build
  end
end
