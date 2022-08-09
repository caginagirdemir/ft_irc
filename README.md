# ft_irc

It is about internet relay chat server through socket programming.

Program run with port and password parameter.

There are 4 different irc command.

- /join #channel -> goes to channel
- /nick #new_nick -> renew nick
- /msg @nickname message -> it send a private message to a user who specify nickname in line
- /list -> shows all available channels

Class functions

void send_message_to_channel(int channel_id, int user_id);

void handle_message(int i);

void disconnect_user(int i);

void check_io_operation();

void check_new_connection();

void init_fds();

void start_listening();

void init_master_server();

bool check_if_command(int i);

void join(std::vector<std::string> params, int i);

void list(std::vector<std::string> params, int i);

void msg(std::vector<std::string> params, int i);

void nick(std::vector<std::string> params, int i);
