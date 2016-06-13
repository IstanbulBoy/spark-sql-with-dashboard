1. Open and build the console application in Visual Studio.
2. Run using below command:
	> Syncfusion.Bigdata.ThriftApplication.exe “Spark-Thrift Server hostname: Port” “Query” 

Example command for executing “Select” query:
	> Syncfusion.Bigdata.ThriftApplication.exe “localhost:10001” “select trips.payment_type, trips.vendor_id, count(*) from (select * from nyctrips_partitionbyyear) trips where trips.payment_type in ('CRD','CSH') group by trips.payment_type, trips.vendor_id”


