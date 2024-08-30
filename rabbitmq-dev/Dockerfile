# Use the RabbitMQ official image with version 3.11.23 and management plugin enabled
FROM rabbitmq:3.11.23-management
USER 0
# Enable all listed plugins using a single command
#RUN rabbitmq-plugins enable rabbitmq_web_stomp rabbitmq_management rabbitmq_stomp rabbitmq_amqp1_0 rabbitmq_shovel #rabbitmq_shovel_management rabbitmq_prometheus rabbitmq_web_stomp_examples rabbitmq_peer_discovery_k8s rabbitmq_federation #rabbitmq_federation_management rabbitmq_tracing
# RUN rabbitmq-plugins enable rabbitmq_prometheus rabbitmq_auth_mechanism_ssl

# Copy custom configuration file to RabbitMQ config directory
ADD ./rabbitmq.conf /etc/rabbitmq/
ADD ./enabled_plugins /etc/rabbitmq/
