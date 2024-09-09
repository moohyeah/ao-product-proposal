| 标题 | 描述 | 作者 | 应用类型 |
|------|------|------|----------|
| Yalla Jamel | 《Yalla Jamel》是一款由Arweave旗下的AO Games推出的全上链三消益智游戏，通关率仅为0.1% | 團隊: WiiGame CEO: 魏大地TEL: +8613016333230Telegram: @wiigameE-mail：451565976@qq.com | 链游|

-----------
# 摘要
《Yalla Jamel》是由Arweave旗下的AO Games推出的全上链三消益智游戏。玩家可以通过消除物品赚取积分，并在Telegram和X平台上与其他玩家实时交流互动。更令人兴奋的是，《Yalla Jamel》实现了游戏内资产与web3钱包的无缝连接，不仅为玩家带来游戏乐趣，还提供了变现和增值资产的机会，真正实现了名利双收。


# 动机
在现有的链游生态中，许多游戏虽然融合了区块链技术，但缺乏创新的游戏玩法和用户互动性，往往使玩家体验停留在纯粹的投机行为上。游戏的核心乐趣与经济价值分离，导致用户粘性不足，留存率低。
《Yalla Jamel》通过三消益智玩法与区块链技术的结合，提供了创新且高度互动的游戏体验。它不仅解决了链游生态中用户缺乏长时间投入和持续参与的痛点，还让玩家通过轻松上手的游戏玩法获得经济回报，促使更多用户愿意参与并留在生态中。这种双重动机——即游戏乐趣和资产增值，正是当前链游生态所急需的。


# 原理及具体可实行性描述
## Game Client 
### Repository: https://github.com/moohyeah/camel
### 1、Use arweave-wallet-kit to integrate AR account login

### 2、Use @permaweb/aoconnect to interact with ao. ao mainly implements the following functions：

   2.1、Query token balance through dryrun

   2.2、At the start of the game, generate a random number sequence via a Play message and return it to the client.

   2.3、After the game is completed, calculate a CheckSum based on the returned random number sequence and the score, then send an Exit message to the server.

### 3、Deploy permaweb using ArDrive

https://app.ardrive.io/#/drives/078a3e9f-5028-48bb-9531-0aae3c23f48b/folders/2d484633-1e57-4d37-a14d-51f468edb477

![Alt text](sc1.jpg?raw=true "Title")

## AO Client
### Process ID：2RLwmjFijKkoRko-9Mr6aJBQFRaV1OB3Q8IeOFNuqRI
### Repository: https://github.com/moohyeah/camelaosvr
### 1、Implement token functionality in token.lua, with reference to the Token Blueprint template.
### 2、game.lua implements server logic, mainly consisting of two handlers.
2.1、Play: Return a random number after the game starts.

![Alt text](sc2.jpg?raw=true "Title")

2.2、Exit: Validate and mint tokens for the player based on their score after completing the game."

![Alt text](sc3.jpg?raw=true "Title")

# 参考实现
[质押蓝图](https://cookbook_ao.g8way.io/zh/guides/aos/blueprints/staking.html)

[permaweb](https://cookbook.arweave.dev/zh/concepts/permawebApplications.html)

# 所需资源（可选）
项目预算: 10000u

permaweb 相关资源
