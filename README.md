# Nitro Gen
## Getting Started
To start you want to download the files as a zip and then unzip it. After that open up Nitro Gen.bat and it will start the program. When the program starts you will have options.
- Gen and Check
- Just Gen
- Just Check
# Genning
While the program is running it will gen codes then save them to the file codes.txt
# Checking
During checking if rate limit occurs it will wait and save the code that was not checked to a file to check them just copy them from notchecked.txt to codes.txt you can delete the other codes and only checked the unused codes. Then run Just Check to check them.
# Getting discord.gift
If you want to add discord.gift you can by making a program with this code then running it.
```javascript
const fs = require('fs')
const codes = fs.readFileSync('./codes.txt').toString().split('\n')

const stream = fs.createWriteStream("./codeswgift.txt", { 'flags': 'a', 'encoding': null, 'mode': 0666})

for(code in codes){
  stream.write('discord.gift/' + codes[code])
  console.log('Wrote')
}
```
