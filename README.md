# BlockEmulator Test

## 运行指令

### 说明

-g、 --gen isGen是一个bool值，表示是否生成批处理文件
-n、 --nodeID int nodeID是一个整数，表示该节点的ID。取值范围：[0，nodeNum）。（默认值-1）
-N、 --nodeNum int nodeNum是一个整数，表示每个分片部署了多少节点。（默认值4）
-s、 --shardID int shardID是一个整数，表示此节点所属的分片的ID。值范围：[0，shardNum）。（默认值-1）
-S、 --shardNum int shardNum是一个整数，表示部署了多少个分片。（默认值4）
-f、 --shellForExe isGenerateForExeFile是一个bool值，只有当“isGen”为true时才有效；为可执行文件生成True，为“go run”生成False。
-c、 --supervisor isSupervisor是一个bool值，表示该节点是否为supervisor。

### 启动

--运行编译脚本: zPrecompileScripts\windows_precomplieScript.sh

--./blockEmulator_Windows_Precompile.exe -g  -N 4  -S 4

-- 测试：go test -v ./query
