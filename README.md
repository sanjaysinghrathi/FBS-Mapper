# FBS-Mapper
preprep

keep original reference file in local directory

./bin/flink run --class org.myorg.avllrmapper.AVLLR_Mapper /target/AVLLR-Mapper.jar a.txt hdfs://localhost:9000/chr.txt hdfs://localhost:9000/chromosome.txt
suffix-prep

cd ..

cd suffix-prep
./bin/flink run --class org.myorg.avllrmapper.AVLLR_Mapper /target/AVLLR-Mapper.jar
suffix-a

cd ..

cd suffix-a
./bin/flink run --class org.myorg.avllrmapper.AVLLR_Mapper /target/AVLLR-Mapper.jar hdfs://localhost:9000/join-reference.txt 50 20 hdfs://localhost:9000/suffixa.txt
