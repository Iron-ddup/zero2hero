## 合约解释说明：

## 第一阶段合约部署

1.首先部署代币合约：AToken
**0xd0f54b3d3D1A52AE08d5e8D4E4D3B6030F752AaE**  

txHash: 0xe62d76ce575daa7a043b8ffbdfd2ea440030c0ee228c383c8f4589e12760c50a

浏览器地址：https://testnet.bscscan.com/token/0xd0f54b3d3D1A52AE08d5e8D4E4D3B6030F752AaE#code

2.部署质押奖励合约：BToken-award

**0x552925E0b2eCeD7558f991FEFDc29500e3B8dBbb**

txHash: 0xb9e8f673801ca92d1b8854f9777000649035d2194b4cdbbf58c1a7ff97c5dc74

3.部署流动性挖矿合约：**LiquidityMiningInitializable**

**0xCCfEd4a0857d02B78Be097602b5654e51EB48811**

txhash: 0x18b91a2b2052b0924abf42d2c702ef86459eee2e22bd2f6d34998dd8d48b416f

token合约地址：
https://github.com/bnb-chain/bsc-genesis-contract/blob/master/contracts/bep20_template/BEP20Token.template

## 第二阶段给合约初始化

0xd0f54b3d3D1A52AE08d5e8D4E4D3B6030F752AaE,0x552925E0b2eCeD7558f991FEFDc29500e3B8dBbb,0x96595d42c28395c5D6994688E7978Dbdb5862f6f,20000,28232300,28888888,0,0x601549c5da78C1773340562F74D75972650D3136

参数介绍看合约注释

到区块28232300高度时开始奖励质押，28888888区块时间结束活动，期间要保持奖励代币足够多



A.调用质押代币合约之前请授权质押合约可以调用你的质押token

txhsah: 0xd065315882d81a06618d085419e2f4d415fceafb46b3c2ac45bd71b303d3eedc

B.质押你的代币等到区块高度到达获取奖励

txhash: 0x08941915cf630134b56fdad59738a9420512ac19a045aa3441417e279c66ccf0

详细交易流程请看账号：
***0x601549c5da78C1773340562F74D75972650D3136***



ps:
一般大家是把代币的token在对应的swap比如pancake swap 上面添加流动性之后，获得配对合约的给它的lp。

最后你质押lp获取空投

上面的测试没做添加流动性这步，没找到test链的swap,原理是一样的。。。。









