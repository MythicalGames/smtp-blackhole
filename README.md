# SMTP Blackhole Container

This container is useful for sending emails during load testing and not having them affect mail provider reputation.

By default it listens on port 1025 with no TLS. It will accept any email address and reply to the requesting service with a 250 OK.

