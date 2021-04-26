# 8xflow-puml-styles

PlantUML 8xFlow theme 
该项目基于 C4 plantUML 修改

## 元素

参考 8xFlow 元素，


#### 时标对象 - 粉红色
类型：RFP，Proposal，Contract(Required)，Fulfillment request - Fulfillment confirmation
时标：时间段(Fulfillment request)，时间点(其他)
关键数据项：时标对象中的关键数据，如，价格
```puml
Rfp(rfp) #RFP
Proposal(proposal) #Proposal
Contract(contract) #合同
Fr(fulfillment_request) #Fulfillment Request
Fc(fulfillment_confirmed) #Fulfillment Confirmed
```

### 参与者 - 绿色
```puml
Party(party, "Party") #参与方：参与人，其他参与者
Thing(thing, "Thing") #标的物(Optional)：权责当事人权利和义务所指向的对象。比如买卖合同中的商品，房屋租赁合同中的房屋。
Place(place, "Place") #场所：合同发生的地方
```

### 角色 -  橙色
```puml
RoleParty(role_party, "RoleParty") #将实际参与方抽象为权利方和责任方
RoleEvidence(evidence_role, "RoleEvidence") #将其他合同中的凭证作为履约凭证，作为变化点，抽象为角色
Role3rdSys(third_sys, "Role3rdSys") #如果三方系统或复杂领域逻辑，通过拟人化手法抽象为角色
``` 

### 边界
```puml
Boundary(boundary_alias, "边界") {
}
```

### 连线
```puml
Rel_x  #实线
Rel_x_dashed #虚线
```
