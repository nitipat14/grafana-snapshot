# grafana-snapshot Package [![Build Status](https://travis-ci.com/ascendcorp/grafana-snapshot.svg?branch=master)](https://travis-ci.com/ascendcorp/grafana-snapshot)


## Install
If you want to use the API algorithms in your code, it is as simple as:

    $ pip install grafana-snapshot

You can test by creating a python file:

```python3
from GrafanaSnapshot.GenerateSnapshot import GenerateSnapshot

if __name__ == "__main__":
    grafana = SnapshotFace(auth='xxxxx', host='localhost', port='3000', protocol='https')
    
    ## Create snaphot
    results = grafana.snapshots.create_snapshot(tags="test_tag", time_from=1563183710618, time_to=1563185212275)
    
    ## Delete snaphot by key
    result = grafana.snapshots.delete(delete_key='some_delete_key', key=None)
```



## Uninstall
If you want to uninstall grafana-snapshot, it is as simple as:

    $ pip uninstall -y grafana-snapshot


## Status

| API | Status |
|---|---|
| Create Snapshot | + |
| Delete Snapshot | + |
| Get Snapshot by tags | - |
