```mermaid
flowchart TB;
		subgraph C端
			web-fe-->web-api;
		end
		subgraph 运营后台
			manage-fe-->manage-api;
		end
		subgraph grpc服务
	    web-api & manage-api --> theme-grpc & factory-grpc;
		end
```
