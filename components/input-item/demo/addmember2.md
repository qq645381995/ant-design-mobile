# 添加店长

- order: 2

列表主体内容的容器。

---

````jsx
import { ListWrap, ListBody, ListFooter, InputItem, ListItem, Button} from 'antm';

ReactDOM.render(
  <div>
  <ListWrap>
    <ListBody>
      <ListItem
        link="http://www.baidu.com"
        extra="请选择"
        arrow="horizontal"
      >所属门店</ListItem>
      <InputItem
        name="yyy"
        clear={true}
        placeholder="真实姓名或昵称"
      >员工姓名</InputItem>
      <InputItem
        name="yyy"
        clear={true}
        placeholder="用作账户名的后缀名"
      >用户名</InputItem>
    </ListBody>
    <ListFooter onClick={function(e){console.log(e);}}>
      账户名：<span style={{'color':'red'}}>zhifubao@alipay.com#用户名</span>
    </ListFooter>
  </ListWrap>
  <ListWrap>
      <ListBody>
        <InputItem
          name="yyy"
          clear={true}
          placeholder="请填写该员工的手机号码"
        >员工手机</InputItem>
        <InputItem
          name="yyy"
          clear={true}
          placeholder="选填"
        >邮箱地址</InputItem>
        <ListItem
          link="http://www.baidu.com"
          arrow="horizontal"
        >员工权限</ListItem>
      </ListBody>
      <ListFooter onClick={function(e){console.log(e);}} style={{'textAlign':'center'}}>拥有退款权限的员工可在交易创建后3天内发起退款</ListFooter>
    </ListWrap>
    <div className="am-wingblank am-wingblank-10">
      <Button mode="blue" type="link">确认添加</Button>
    </div>
  </div>
, document.getElementById('components-input-item-demo-addmember2'));
````