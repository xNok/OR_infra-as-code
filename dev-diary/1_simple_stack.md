Simple Stack
---

Given that most OR-scientist or not system operators (OPS) it seems more believable to rely on Docker rather than Kubernetes. Either way ultimately we are only running ephemaral docker container at edge and a couple docker on the master node for assets and datamanagement .

## Partitioning the disk of the master node (Optional)


| Type | fs type | mount | Size      |
|------|---------|-------|-----------|
|primary |	ext4 | /boot |	512 MB	 |	
|primary |	ext4 | /	 |  20000 MB |		
|primary |	ext4 | /home |	20000 MB |		
|primary |	swap | swap	 |  512 MB	 |	
|primary |	ext4 | /data |	Remain   |	