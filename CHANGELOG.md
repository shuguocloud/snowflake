# snowflake Changelog

1. snowflake添加go.mod

2. 测试 TestNewNode
    
   go test -v -run="TestNewNode"

   === RUN   TestNewNode
   --- PASS: TestNewNode (0.00s)
   PASS
   ok      github.com/shuguocloud/snowflake        0.038s

   go test -v -run="TestPrintAll"
   
   === RUN   TestPrintAll
       TestPrintAll: snowflake_test.go:73: Int64    : 2354207071928320
       TestPrintAll: snowflake_test.go:74: String   : "2354207071928320"
       TestPrintAll: snowflake_test.go:75: Base2    : "1000010111010010001110001100010000000000000000000000"
       TestPrintAll: snowflake_test.go:76: Base32   : "nn7rqgryyyy"
       TestPrintAll: snowflake_test.go:77: Base36   : "n6hvsqstts"
       TestPrintAll: snowflake_test.go:78: Base58   : "joe2BkTAq"
       TestPrintAll: snowflake_test.go:79: Base64   : "MjM1NDIwNzA3MTkyODMyMA=="
       TestPrintAll: snowflake_test.go:80: Bytes    : []byte{0x32, 0x33, 0x35, 0x34, 0x32, 0x30, 0x37, 0x30, 0x37, 0x31, 0x39, 0x32, 0x38, 0x33, 0x32, 0x30}
       TestPrintAll: snowflake_test.go:81: IntBytes : [8]uint8{0x0, 0x8, 0x5d, 0x23, 0x8c, 0x40, 0x0, 0x0}
   --- PASS: TestPrintAll (0.00s)
   PASS
   ok      github.com/shuguocloud/snowflake        0.031s
