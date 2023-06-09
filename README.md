
{
    "vectors": {
      "size": 1024,
      "distance": "Euclid"
    },
    "quantization_config": {
        "scalar": {
            "type": "int8",
            "quantile": 0.99,
            "always_ram": true
        },
        "product": {
            "compression": "x16",
            "always_ram": true
        }
    }
}

{
    "result": {
        "status": "green",
        "optimizer_status": "ok",
        "vectors_count": 0,
        "indexed_vectors_count": 0,
        "points_count": 0,
        "segments_count": 8,
        "config": {
            "params": {
                "vectors": {
                    "size": 4,
                    "distance": "Dot"
                },
                "shard_number": 1,
                "replication_factor": 1,
                "write_consistency_factor": 1,
                "on_disk_payload": true
            },
            "hnsw_config": {
                "m": 16,
                "ef_construct": 100,
                "full_scan_threshold": 10000,
                "max_indexing_threads": 0,
                "on_disk": false
            },
            "optimizer_config": {
                "deleted_threshold": 0.2,
                "vacuum_min_vector_number": 1000,
                "default_segment_number": 0,
                "max_segment_size": null,
                "memmap_threshold": null,
                "indexing_threshold": 20000,
                "flush_interval_sec": 5,
                "max_optimization_threads": 1
            },
            "wal_config": {
                "wal_capacity_mb": 32,
                "wal_segments_ahead": 0
            },
            "quantization_config": null
        },
        "payload_schema": {}
    },
    "status": "ok",
    "time": 0.000076592
}
