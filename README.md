process-logger
============

kills the previous process of this application

## Install

```
git clone https://github.com/mixamarciv/process-logger.git
```

## Usage

```js
//run and show process info
p = { run: 'test.bat',
      log: 'file.log',
      args: ['argument1', 'arg2'],
      enc: 'cp866',
      on_data: function(data){console.log(data);},
      out_stream: fs.createWriteStream('out.file')
    }
process_logger(p,function(err,exit_code){
    console.log('child process exited with code ' + exit_code);
});

```




## License
MIT
