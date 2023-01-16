# NFT_study
- Non-Fungible Token (NFT): 非代替性トークン
- fungible: (取引などで)代替・交換可能な
---


## 規格 EIP, ERC とは
- https://eips.ethereum.org/EIPS/eip-1
- Ethereum Improvement Proposal (EIP): イーサリアムの改善提案
- EIP types: Standards Track EIP, Meta EIP, Information EIP
- Standard EIP: Core, Networking, Interface, ERC
- NFTはERCの721番目の提案のため、ERC-721 と呼ばれたりする

 
## ERC-721: Non-Fungible Token Standard
- https://eips.ethereum.org/EIPS/eip-721

### 内容
- NFTを追跡可能にするための機能提供が目的の標準API規定
- NFTコントラクトアドレスとトークンIDをセットで管理している
- 
        NFTコントラクトアドレス
        |
        |--- トークンID1
        |--- トークンID2
        ...
- トークンIDにコンテンツを紐づけることができる（絵とか、資産全般いける）
  - 具体的には、JSON形式のメタデータを紐づける
  - メタデータにコンテンツへのURIを設定
    - 例えば　OpenSea のメタデータのスタンダード
    - https://docs.opensea.io/docs/metadata-standards#metadata-structure
  - メタデータの紐づけはオプション機能で、必須ではない
  - [ ] URIを直接変更されると管理できない？　コンテンツはどこに存在するべきなんだ？
    - ブロックチェーン内には無理そう、容量なさそうだしガス高くなりそう

### Ethereumについて
- データの持ち様
- https://www.lucassaldanha.com/ethereum-yellow-paper-walkthrough-2/