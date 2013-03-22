riak_kv_wm_search_stats
=======================

Quick and dirty way to expose search stats via /search_stats

### How to build

1) Check out riak source, make ( to download deps )

2) riak_kv.patch: use this to patch riak_kv in deps

3) riak_kv_wm_search_stats.erl: add to deps/riak_kv/src

4) make rel

### To deploy on already installed riak ( i.e. installed via package, etc )
1) copy deps/riak_kv/ebin/riak_kv_web.beam & deps/riak_kv/ebin/riak_kv_wm_search_stats.beam into /usr/lib*../basho-patches

2) restart riak

3) browse to http://localhost:8098/search_stats