English | [繁體中文](./README.zh-TW.md)

# ZbxTable

ZbxTable is a Zabbix report system developed using Go language.

## Features

- Export detailed data and trend data of monitoring indicators in a specific time period to xlsx files.
- Export Zabbix alarm messages to xlsx files in a specific time period.
- Alarms are analyzed for a specific time period of the message, for example, alarms and the like Top10.
- Export inspection report according to host group.
- Display and view Zabbix graphics according to the host and support export to pdf.
- Display of host status and unrecovered alarm information.

## Architecture

![1](https://img.cactifans.com/wp-content/uploads/2020/07/zbxtable.png)

## Component

ZbxTable: Backend written using [beego framework](https://github.com/astaxie/beego).

ZbxTable-Web: Front end written using [React](https://github.com/facebook/react).

MS-Agent: Installed on Zabbix Server, used to receive alarms generated by Zabbix Server and send to ZbxTable.

## Demo

[https://zbx.cactifans.com](https://zbx.cactifans.com)

## Compatibility

| Zabbix Version | Compatibility |
| :------------- | :------------ |
| 5.4.x          | ✅            |
| 5.2.x          | ✅            |
| 5.0.x LTS      | ✅            |
| 4.4.x          | ✅            |
| 4.2.x          | ✅            |
| 4.0.x LTS      | ✅            |
| 3.4.x          | ✅            |
| 3.2.x          | ✅            |
| 3.0.x LTS      | ✅            |

## Documentation

[ZbxTable Documentation](https://zbxtable.cactifans.com)

## Code

**ZbxTable**: [https://github.com/canghai908/zbxtable](https://github.com/canghai908/zbxtable)

**ZbxTable-Web**: [https://github.com/canghai908/zbxtable-web](https://github.com/canghai908/zbxtable-web)

**MS-Agent**: [https://github.com/canghai908/ms-agent](https://github.com/canghai908/ms-agent)

## Compile

```
mkdir -p $GOPATH/src/github.com/canghai908
cd $GOPATH/src/github.com/canghai908
git clone https://github.com/canghai908/zbxtable.git
cd zbxtable
./control build
./control pack
```

## Team

Back-end development

[canghai908](https://github.com/canghai908)

Front-end development

[ahyiru](https://github.com/ahyiru)

## License

<img alt="Apache-2.0 license" src="https://s3-gz01.didistatic.com/n9e-pub/image/apache.jpeg" width="128">

ZbxTable is available under the Apache-2.0 license. See the [LICENSE](LICENSE) file for more info.
