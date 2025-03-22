# multi-duckdb-demo
multi-duckdb-demo
![image](https://github.com/user-attachments/assets/01839042-8d57-4774-9db5-c5101c3a1223)


Create a Virtual Environment
```
virtualenv -p python3.10 myenv
cd /Users/soumilshah/IdeaProjects/icebergpython/Arrow/lab7/
source myenv/bin/activate
```

Clone the Project
```
git clone git@github.com:soumilshah1995/xorq.git
cd xorq
git checkout dan/examples/multi-duck
pip install -e .

```

Run DuckDB Flight RPC Example
```
python3 examples/duckdb_flight_example.py \
    serve \
    -p 8816 \
    -d multi.db \
    -n test


python3  examples/duckdb_flight_example.py \
    write \
    -p 8816 \
    -d multi.db \
    -n test


python3   examples/duckdb_flight_example.py \
    read \
    -p 8816 \
    -d multi.db \
    -n test
```
