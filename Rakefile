# frozen_string_literal: true

require "bundler/gem_tasks"
require_relative "lib/ruby_play/version"
task default: %i[]



task :compare_versions, [:github_ref] do |t, args|
    unless args.github_ref.end_with?(RubyPlay::VERSION)
        abort("version mismatch between GITHUB_REF=#{args.github_ref} and gem veriosn=#{RubyPlay::VERSION}")
    else
        puts "gem version #{RubyPlay::VERSION} matched with GITHUB_REF"
    end
end


task :get_version do |t|
    puts RubyPlay::VERSION
end                                                                                                                   