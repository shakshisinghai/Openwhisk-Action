# Openwhisk-Action

Turn of Hyper V
```
bcdedit
bcdedit /set hypervisorlaunchtype auto
```

```
 sudo docker build -t ssingha2/openwhisk-ml_docker .
 
 sudo docker tag python3action:ml-libs ssingha2/python3action:ml-libs
 
 sudo docker push ssingha2/python3action:ml-libs
 
 wsk -i action create ml-libs --docker ssingha2/python3action:ml-libs action.py
 
 wsk -i action invoke ml-libs --result
 
 wsk -i activation get (id)
 ```
