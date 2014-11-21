require 'webrick'

class Default < Thor
  desc 'serve', 'Serve the boilerplate html page for previewing purposes'
  def serve
    config = {
      Port: 1234,
      DocumentRoot: "#{Dir.pwd}"
    }
    server = WEBrick::HTTPServer.new(config)

    ['INT', 'TERM'].each { |signal| trap(signal) { server.shutdown } }

    server.start
  end
end
