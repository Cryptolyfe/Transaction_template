# transaction_template
A general template for a blockchain transaction




const Web3 = require('web3')
const rpcURL = 'http://127.0.0.1:7545'
const web3 = new Web3(rpcURL)

const account1 = "0x043..."
const account2 = "0x087..."

web3.eth.sendTransaction({
  from: account1,
  to: account2,
  value: web3.utils.toWei('1', 'ether')
},
(err, result)
 => {
   console.log(result)
 }
})
