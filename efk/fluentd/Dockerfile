# fluentd/Dockerfile
FROM fluent/fluentd:v0.12-debian
RUN ["gem", "install", "fluent-plugin-elasticsearch", "--no-rdoc", "--no-ri", "--version", "1.9.2"]
RUN ["gem", "install", "fluent-plugin-nsca"]
RUN ["cp", "-vf", "/usr/share/zoneinfo/Europe/Riga", "/etc/localtime"]
RUN ["echo", "Europe/Riga", "|", "tee", "/etc/timezone"]
