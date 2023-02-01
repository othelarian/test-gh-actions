fs = require 'fs'
pug = require 'pug'

task 'github', '', (_) ->
  try
    fs.mkdirSync 'docs', { recursive: true }
    out = pug.renderFile 'index.pug'
    fs.writeFileSync 'docs/index.html', out
  catch e
    console.log "error:\n#{e}"