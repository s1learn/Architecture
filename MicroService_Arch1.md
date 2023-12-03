graph TD

  subgraph LegacyApplication
    LA1(Legacy App with .NET Framework 4.7)
    LA2(Grapecity ActiveReports)
  end
  LA1 ---> LA2
  
  subgraph LegacyApplication
    LA1(Legacy App with .NET Framework 4.7)
    LA2(Grapecity ActiveReports)
  end

  subgraph Browser
    MFE1(Micro Frontend 1)
    MFE2(Micro Frontend 2)
  end

  subgraph IntegrationEngine
    IE(Integration Engine)
  end

  subgraph Microservices
    MS1(Microservice 1)
    MS2(Microservice 2)
    MS3(Microservice 3)
  end

  subgraph Database
    DB1(DB 1)
    DB2(DB 2)
    DB3(DB 3)
  end

  MFE1 --> IE
  MFE2 --> IE
  IE --> MS1
  IE --> MS2
  IE --> MS3
  MS1 --> DB1
  MS2 --> DB2
  MS3 --> DB3
