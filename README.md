gitbook 见 ：https://socket.gitbook.io/docs/

# Socket.io 文档中文翻译项目

在过去，曾多次使用到socket.io，但也仅仅是使用基础的模块。最近因为自己做了一个比较大的消息推送架构，再次使用到了socket.io，不由的感慨，这真是一个优秀的社区项目。

为了更加深入学习和使用socket.io，现在我把它的文档中文翻译下，也方便自己学习。

## TODO
> 剩下API 尚未完成

## 目录

- [关于本socket.io中文文档](README.md)
- [Guide]()
    - [介绍](guide/1-introduction.md)
    - [web框架](guide/2-the_web_framework.md)
    - [服务HTML](guide/3-serving_html.md)
    - [集成 socket.io](guide/4-integrating_socket.io.md)
    - [发送事件](guide/5-emitting_events.md)
    - [广播](guide/6-broadcasting.md)
    - [作业](guide/7-homework.md)
    - [获取示例](guide/8-getting_this_example.md)

- [Documents]()
    - [overview]()
        - [what_socket.io_is](docs/overview/what_socket.io_is.md)    
        - [what_socket.io_is_not](docs/overview/what_socket.io_is_not.md)    
        - [installing](docs//overview/installing.md)    
        - [using_with_node_http_server](docs/overview/using_with_node_http_server.md)    
        - [using_with_express](docs/overview/.md)    
        - [sending_and_receiving_events](docs/overview/sending_and_receiving_events.md)    
        - [restricting_yourself_to_a_namespace](docs/overview/restricting_yourself_to_a_namespace.md)    
        - [sending_volatile_message](docs/overview/sending_volatile_message.md)    
        - [sending_and_getting_data_acknowledgements](docs/overview/sending_and_getting_data_acknowledgements.md)  
        - [broadcasting_messages](docs/overview/broadcasting_messages.md)   
        - [using_it_just_as_a_cross_browser_websocket](docs/overview/using_it_just_as_a_cross_browser_websocket.md)     
    - [rooms_and_namespaces]()
    - [migrating_from_0.9]()
    - [using_multiple_nodes]()
    - [logging_and_debugging]()
    - [emit_cheatsheet](docs/emit_cheatsheet.md)
    - [internals_overview]()
        - [internals_overview_dependency_graph_under_the_hood](docs/internals_overview_dependency_graph_under_the_hood.md)
        - [internals_overview_dependency_graph](docs/internals_overview_dependency_graph.md)
     - [faq](docs/faq.md)   

- [Client-API]()
    - [io]()
        - [io.protocpl](io_protocol.md)
        - [io([url][,optiosn])](io_url_options.md)
        - [初始化示例-带多路复用](initialization_examples_with_multiplexing.md)
        - [初始化示例-自定义路径](initialization_examples_with_custom_path.md)
        - [初始化示例-查询参数](initialization_examples_with_query_parameters.md)
        - [初始化示例-查询选项](initialization_examples_with_query_option.md)
        - [初始化示例-额外Headers](initialization_examples_with_extraHeaders.md)
        - [初始化示例-仅限websocket传输](initialization_examples_with_websockets_transport_only.md)
        - [初始化示例-自定义解析器](initialization_examples_with_a_custom_parser.md)
        - [初始化示例-自签名](initialization_examples_with_a_self-signed.md)
        - [初始化示例-证书](initialization_examples_certificate.md)

    - [manager]()
        - [new Manager(url[,options])](new_manager_url_options.md)
        - [manager.reconnection([value])](manager_reconnection_value.md)
        - [manager.reconnectionAttempts([value])](manager_reconnectionAttempts_value.md)
        - [manager.reconnectionDelay.([value])](manager_reconnectionDelay_value.md)
        - [manager.reconnectionDelayMax([value])](manager_reconnectionDelayMax_value.md)
        - [manager.timeout(pvalue[])](manager_timeout_value.md)
        - [manager.open([callback])](manager_open_callback.md)
        - [manager.connect([callback])](manager_connect_callback.md)
        - [manager.socket(nsp,options)](manager_socket_nsp_options.md)
        - [event:connect_error](event_connect_error.md)
        - [event:connect_timeout](event_connect_timeout.md)
        - [event:reconnect](event_reconnect.md)
        - [event:reconnect_attempt](event_reconnect_attempt.md)
        - [event:reconnecting](event_reconnecting.md)
        - [event:reconnect_error](event_reconnect_error.md)
        - [event:reconnect_failed](event_reconnect_failed.md)
        - [event:ping](event_ping.md)
        - [event:pong](event_pong.md)

    - [socket]()
        - [socket.id](socket_id.md)
        - [socket.connected](socket_connected.md)
        - [socket.disconnected](socket_disconnected.md)
        - [socket.open()](socket_open.md)
        - [socket.connect()](socket_connect.md)
        - [socket.send([...args][,ack])](socket_send_args_ack.md)
        - [socket.emit(eventName,[...args][,ack])](socket_emit_eventName_args_ack.md)
        - [socket.on(eventName,callback)](socket_on_eventName_callback.md)
        - [socket.compress(value)](socket_compress_value.md)
        - [socket.binary(value)](socket_binary_value.md)
        - [socket.close()](socket_close.md)
        - [socket.disconnect()](socket_disconnect.md)
        - [event:connect](event_connect.md)
        - [event:connect_error](event_connect_error.md)
        - [event:connect_timeout](event_connect_timeout.md)
        - [event:error](event_error.md)
        - [event:disconnect](event_disconnect.md)
        - [event:reconnect](event_reconnect.md)
        - [event:reconnect_attempt](event_reconnect_attempt.md)
        - [event:reconnenting](event_reconnenting.md)
        - [event:reconnect_error](event_reconnect_error.md)
        - [event:reconnect_failed](event_reconnect_failed.md)
        - [event:ping](event_ping.md)
        - [event:pong](event_pong.md)

- [Server-API]()

    - [server]()
        - [new_server_httpserver_options](new_server_httpserver_options.md)
        - [new_server_port_options](new_server_port_options.md)
        - [new_server_options](new_server_options.md)
        - [server_sockets](server_sockets.md)
        - [server_serverClient_value](server_serverClient_value.md)
        - [server_path_value](server_path_value.md)
        - [server_adapter_value](server_adapter_value.md)
        - [server_origins_value](server_origins_value.md)
        - [server_origins_fn](server_origins_fn.md)
        - [server_attach_port_options](server_attach_port_options.md)
        - [server_listen_httpServer_options](server_listen_httpServer_options.md)
        - [server_listent_port_options](server_listent_port_options.md)
        - [server_bind_engine](server_bind_engine.md)
        - [server_onconnection_socket](server_onconnection_socket.md)
        - [server_of_nsp](server_of_nsp.md)
        - [server_close_callback](server_close_callback.md)
        - [server_engine_generateid](server_engine_generateid.md)

    - [namespace]()
        - [namespace_name](namespace_name.md)
        - [namespace_connectid](namespace_connectid.md)
        - [namespace_adapter](namespace_adapter.md)
        - [namespace_to_room](namespace_to_room.md)
        - [namespace_in_room](namespace_in_room.md)
        - [namespace_emit_eventname_args](namespace_emit_eventname_args.md)
        - [namespace_clients_callback](namespace_clients_callback.md)
        - [namespace_use_fn](namespace_use_fn.md)
        - [event_connect](event_connect.md)
        - [event_connection](event_connection.md)
        - [flag_volatile](flag_volatile.md)
        - [flag_binary](flag_binary.md)
        - [flag_local](flag_local.md)
        
    - [socket]()
        - [socket_id](socket_id.md)
        - [socket_rooms](socket_rooms.md)
        - [socket_client](socket_client.md)
        - [socket_conn](socket_conn.md)
        - [socket_request](socket_request.md)
        - [socket_handshake](socket_handshake.md)
        - [socket_use_fn](socket_use_fn.md)
        - [socket_send_args_ack](socket_send_args_ack.md)
        - [socket_emit_eventName_args_ack](socket_emit_evenName_args_ack.md)
        - [socket_on_eventName_callback](socket_on_eventName_callback.md)
        - [socket_once_eventName_listener](socket_once_eventName_listener.md)
        - [socket_removelistener_eventName_listener](socket_removelistener_eventName_listener.md)
        - [socket_removeAllListeners_eventName](socket_removeAllListeners_eventName.md)
        - [socket_eventNames](socket_eventNames.md)
        - [socket_join_room_callback](socket_join_room_callback.md)
        - [socket_join_rooms_callback](socket_join_rooms_callback.md)
        - [socket_leave_room_callback](socket_leave_room_callback.md)
        - [socket_to_room](socket_to_room.md)
        - [socket_in_room](socket_in_room.md)
        - [socket_compress_value](socket_compress_value.md)
        - [socket_disconnect_close](socket_disconnect_close.md)
        - [flag_broadcast](flag_broadcast.md)
        - [flag_volatile](flag_volatile.md)
        - [flag_binary](flag_binary.md)
        - [event_disconnect](event_disconnect.md)
        - [event_error](event_error.md)
        - [event_disconnecting](event_disconnecting.md)
    - [client]()
        - [client_conn]( client_conn.md  )
        - [client_request](client_request.md)

_________________________________________

by @veaba

2019年3月13日13:39:15

