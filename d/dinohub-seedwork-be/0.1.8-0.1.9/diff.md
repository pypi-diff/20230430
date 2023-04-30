# Comparing `tmp/dinohub_seedwork_be-0.1.8.tar.gz` & `tmp/dinohub_seedwork_be-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinohub_seedwork_be-0.1.8.tar", max compression
+gzip compressed data, was "dinohub_seedwork_be-0.1.9.tar", max compression
```

## Comparing `dinohub_seedwork_be-0.1.8.tar` & `dinohub_seedwork_be-0.1.9.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0     1074 2022-12-16 09:09:54.053571 dinohub_seedwork_be-0.1.8/LICENSE
--rw-r--r--   0        0        0      155 2022-12-16 09:09:54.022652 dinohub_seedwork_be-0.1.8/README.md
--rw-r--r--   0        0        0       26 2022-12-23 11:13:56.668882 dinohub_seedwork_be-0.1.8/dino_seedwork_be/__init__.py
--rw-r--r--   0        0        0      134 2022-12-23 10:25:34.977531 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/__init__.py
--rw-r--r--   0        0        0       86 2022-12-23 11:14:33.893228 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/dto.py
--rw-r--r--   0        0        0      221 2022-12-23 10:24:57.376557 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/logger.py
--rw-r--r--   0        0        0       48 2022-12-23 06:59:49.199000 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/__init__.py
--rw-r--r--   0        0        0      310 2022-12-23 10:05:50.540404 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/firebase/AbstractUserNotificationPushDrivingAdapter.py
--rw-r--r--   0        0        0      876 2022-12-27 08:54:50.998107 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/firebase/FirebaseNotificationDrivingAdapter.py
--rw-r--r--   0        0        0      108 2022-12-23 10:07:14.381257 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/firebase/__init__.py
--rw-r--r--   0        0        0     8763 2022-12-23 10:09:15.078993 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/BrokerComponent.py
--rw-r--r--   0        0        0     2094 2022-12-23 10:09:31.175969 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/ConnectionSettings.py
--rw-r--r--   0        0        0     3193 2022-12-23 10:09:54.305433 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/Exchange.py
--rw-r--r--   0        0        0     5298 2022-12-23 10:10:10.506117 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/ExchangeListener.py
--rw-r--r--   0        0        0    10717 2022-12-23 10:10:28.653802 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/MessageConsumer.py
--rw-r--r--   0        0        0     4147 2022-12-23 10:10:39.921907 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/MessageListener.py
--rw-r--r--   0        0        0     1803 2022-12-23 10:10:51.188641 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/MessageParameters.py
--rw-r--r--   0        0        0     8014 2022-12-23 10:11:07.523388 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/MessageProducer.py
--rw-r--r--   0        0        0      116 2022-12-23 10:11:22.215423 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/MessageType.py
--rw-r--r--   0        0        0    11445 2022-12-23 10:11:39.774950 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/Queue.py
--rw-r--r--   0        0        0     1076 2022-12-23 10:14:04.069478 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/__init__.py
--rw-r--r--   0        0        0      136 2022-12-23 10:09:44.676190 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/exceptions.py
--rw-r--r--   0        0        0     9291 2022-12-23 10:14:27.944113 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/pubsub/RabbitMQPublisher.py
--rw-r--r--   0        0        0       33 2022-12-23 10:14:38.673804 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/pubsub/__init__.py
--rw-r--r--   0        0        0     2524 2022-12-23 10:25:11.851014 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/repository.py
--rw-r--r--   0        0        0       21 2022-12-23 10:22:29.776198 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/rest/__init__.py
--rw-r--r--   0        0        0       82 2022-12-23 10:15:33.452083 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/rest/fastapi/__init__.py
--rw-r--r--   0        0        0      826 2022-12-23 10:14:58.693267 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/rest/fastapi/basic_handle_exception.py
--rw-r--r--   0        0        0      666 2022-12-23 10:15:10.672448 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/rest/fastapi/filters.py
--rw-r--r--   0        0        0      586 2022-12-23 10:15:22.475200 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/rest/fastapi/order.py
--rw-r--r--   0        0        0     5861 2022-12-23 10:22:03.820241 dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/rest/utils.py
--rw-r--r--   0        0        0     3818 2022-12-23 10:25:53.931308 dinohub_seedwork_be-0.1.8/dino_seedwork_be/application/AbstractApplicationLifeCycle.py
--rw-r--r--   0        0        0      500 2022-12-23 10:28:40.509858 dinohub_seedwork_be-0.1.8/dino_seedwork_be/application/ApplicationLifeCycleUseCase.py
--rw-r--r--   0        0        0      177 2022-12-23 10:29:52.819577 dinohub_seedwork_be-0.1.8/dino_seedwork_be/application/__init__.py
--rw-r--r--   0        0        0       48 2022-12-23 10:28:51.608420 dinohub_seedwork_be-0.1.8/dino_seedwork_be/application/command.py
--rw-r--r--   0        0        0      594 2022-12-23 10:29:01.709755 dinohub_seedwork_be-0.1.8/dino_seedwork_be/application/handler.py
--rw-r--r--   0        0        0      313 2022-12-23 10:29:14.588549 dinohub_seedwork_be-0.1.8/dino_seedwork_be/application/query.py
--rw-r--r--   0        0        0      463 2022-12-23 10:29:30.705966 dinohub_seedwork_be-0.1.8/dino_seedwork_be/application/service.py
--rw-r--r--   0        0        0     1132 2022-12-23 10:30:09.907783 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/AbstractDomainEventDict.py
--rw-r--r--   0        0        0     1246 2022-12-26 03:24:07.967231 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/AbstractIdentity.py
--rw-r--r--   0        0        0      258 2022-12-25 16:27:09.922531 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/AggregateRoot.py
--rw-r--r--   0        0        0     2881 2022-12-23 10:30:43.411019 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/DomainEvent.py
--rw-r--r--   0        0        0     3327 2022-12-26 03:15:53.174620 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/DomainEventPublisher.py
--rw-r--r--   0        0        0      414 2022-12-25 16:27:25.542484 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/DomainEventSubscriber.py
--rw-r--r--   0        0        0      323 2022-12-23 10:31:17.425301 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/DomainService.py
--rw-r--r--   0        0        0     1811 2022-12-23 10:31:29.392877 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/Entity.py
--rw-r--r--   0        0        0      973 2022-12-23 10:32:18.225122 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/IdentifiedDomainObject.py
--rw-r--r--   0        0        0      405 2022-12-23 10:32:36.045815 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/IdentifiedValueObject.py
--rw-r--r--   0        0        0     1373 2022-12-23 10:33:04.642067 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/RegexValue.py
--rw-r--r--   0        0        0      438 2022-12-26 04:04:58.780387 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/__init__.py
--rw-r--r--   0        0        0     1083 2022-12-23 10:31:54.292011 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/exceptions.py
--rw-r--r--   0        0        0      760 2022-12-23 10:32:52.407487 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/mixins.py
--rw-r--r--   0        0        0      528 2022-12-23 10:33:17.602347 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/rules.py
--rw-r--r--   0        0        0      244 2022-12-23 10:33:31.882913 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/utils.py
--rw-r--r--   0        0        0      561 2022-12-23 10:36:48.237292 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/validator.py
--rw-r--r--   0        0        0     7300 2022-12-23 10:37:52.263631 dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/value_objects.py
--rw-r--r--   0        0        0     1002 2022-12-23 10:40:12.888448 dinohub_seedwork_be-0.1.8/dino_seedwork_be/event/EventSerializer.py
--rw-r--r--   0        0        0      967 2022-12-23 10:40:24.388207 dinohub_seedwork_be-0.1.8/dino_seedwork_be/event/EventStore.py
--rw-r--r--   0        0        0     2324 2022-12-23 10:41:18.136972 dinohub_seedwork_be-0.1.8/dino_seedwork_be/event/StoredEvent.py
--rw-r--r--   0        0        0      111 2022-12-23 10:43:15.422718 dinohub_seedwork_be-0.1.8/dino_seedwork_be/event/__init__.py
--rw-r--r--   0        0        0     3505 2022-12-23 10:41:50.025534 dinohub_seedwork_be-0.1.8/dino_seedwork_be/event/persistance/SqlAlchemyEventStore.py
--rw-r--r--   0        0        0     3194 2022-12-23 10:42:35.569574 dinohub_seedwork_be-0.1.8/dino_seedwork_be/event/persistance/SqlAlchemyPublishedNotificationTrackerStore.py
--rw-r--r--   0        0        0       95 2022-12-23 10:42:52.507948 dinohub_seedwork_be-0.1.8/dino_seedwork_be/event/persistance/__init__.py
--rw-r--r--   0        0        0     2659 2022-12-23 11:13:46.604360 dinohub_seedwork_be-0.1.8/dino_seedwork_be/exceptions.py
--rw-r--r--   0        0        0       20 2022-12-23 11:14:34.124431 dinohub_seedwork_be-0.1.8/dino_seedwork_be/fp/__init__.py
--rw-r--r--   0        0        0      117 2022-12-23 10:43:39.692868 dinohub_seedwork_be-0.1.8/dino_seedwork_be/fp/list.py
--rw-r--r--   0        0        0       59 2022-12-23 10:44:54.519439 dinohub_seedwork_be-0.1.8/dino_seedwork_be/logic/__init__.py
--rw-r--r--   0        0        0    12044 2022-12-23 10:44:30.578472 dinohub_seedwork_be-0.1.8/dino_seedwork_be/logic/assertion_concern.py
--rw-r--r--   0        0        0      455 2022-12-23 10:44:44.020251 dinohub_seedwork_be-0.1.8/dino_seedwork_be/logic/validators.py
--rw-r--r--   0        0        0     3079 2022-12-23 10:45:15.092145 dinohub_seedwork_be-0.1.8/dino_seedwork_be/media/AbstractJsonMediaReader.py
--rw-r--r--   0        0        0      159 2022-12-23 10:45:25.503373 dinohub_seedwork_be-0.1.8/dino_seedwork_be/media/RepresentationReader.py
--rw-r--r--   0        0        0       75 2022-12-23 10:48:05.944147 dinohub_seedwork_be-0.1.8/dino_seedwork_be/media/__init__.py
--rw-r--r--   0        0        0     1269 2022-12-23 10:48:26.164692 dinohub_seedwork_be-0.1.8/dino_seedwork_be/process/AbstractProcess.py
--rw-r--r--   0        0        0     2067 2022-12-23 10:48:37.130877 dinohub_seedwork_be-0.1.8/dino_seedwork_be/process/AbstractProcessApplicationService.py
--rw-r--r--   0        0        0      718 2022-12-23 10:48:49.228378 dinohub_seedwork_be-0.1.8/dino_seedwork_be/process/ProcessId.py
--rw-r--r--   0        0        0     1621 2022-12-23 10:48:59.326673 dinohub_seedwork_be-0.1.8/dino_seedwork_be/process/ProcessTimeOut.py
--rw-r--r--   0        0        0     8616 2022-12-23 10:49:08.962194 dinohub_seedwork_be-0.1.8/dino_seedwork_be/process/TimeConstrainedProcessTracker.py
--rw-r--r--   0        0        0     1316 2022-12-23 10:49:19.029644 dinohub_seedwork_be-0.1.8/dino_seedwork_be/process/TimeConstrainedProcessTrackerRepository.py
--rw-r--r--   0        0        0      272 2022-12-23 10:50:14.910034 dinohub_seedwork_be-0.1.8/dino_seedwork_be/process/__init__.py
--rw-r--r--   0        0        0      783 2022-12-23 10:49:28.772379 dinohub_seedwork_be-0.1.8/dino_seedwork_be/process/timeout_event_factory.py
--rw-r--r--   0        0        0     1129 2022-12-23 10:50:27.096845 dinohub_seedwork_be-0.1.8/dino_seedwork_be/pubsub/DefaultImplementNotificationApplicationService.py
--rw-r--r--   0        0        0     3112 2022-12-23 10:50:42.899716 dinohub_seedwork_be-0.1.8/dino_seedwork_be/pubsub/Notification.py
--rw-r--r--   0        0        0      886 2022-12-23 10:50:54.376921 dinohub_seedwork_be-0.1.8/dino_seedwork_be/pubsub/NotificationPublisher.py
--rw-r--r--   0        0        0     1689 2022-12-23 10:58:52.492569 dinohub_seedwork_be-0.1.8/dino_seedwork_be/pubsub/NotificationReader.py
--rw-r--r--   0        0        0     1173 2022-12-23 10:59:07.835347 dinohub_seedwork_be-0.1.8/dino_seedwork_be/pubsub/NotificationSerializer.py
--rw-r--r--   0        0        0     3195 2022-12-23 10:59:20.557003 dinohub_seedwork_be-0.1.8/dino_seedwork_be/pubsub/PublishedNotificationTracker.py
--rw-r--r--   0        0        0     1138 2022-12-23 10:59:32.477207 dinohub_seedwork_be-0.1.8/dino_seedwork_be/pubsub/PublishedNotificationTrackerStore.py
--rw-r--r--   0        0        0      292 2022-12-23 11:00:15.454131 dinohub_seedwork_be-0.1.8/dino_seedwork_be/pubsub/__init__.py
--rw-r--r--   0        0        0        0 2022-12-26 04:06:29.307336 dinohub_seedwork_be-0.1.8/dino_seedwork_be/py.typed
--rw-r--r--   0        0        0      163 2022-12-23 11:00:28.079371 dinohub_seedwork_be-0.1.8/dino_seedwork_be/serializer/AbstractSerializer.py
--rw-r--r--   0        0        0      838 2022-12-23 11:00:39.676133 dinohub_seedwork_be-0.1.8/dino_seedwork_be/serializer/ObjectSerializer.py
--rw-r--r--   0        0        0      365 2022-12-23 11:00:50.758546 dinohub_seedwork_be-0.1.8/dino_seedwork_be/serializer/Serializable.py
--rw-r--r--   0        0        0       94 2022-12-23 11:01:45.872572 dinohub_seedwork_be-0.1.8/dino_seedwork_be/serializer/__init__.py
--rw-r--r--   0        0        0       19 2022-12-23 11:03:42.645054 dinohub_seedwork_be-0.1.8/dino_seedwork_be/storage/__init__.py
--rw-r--r--   0        0        0     5318 2022-12-27 09:07:44.119207 dinohub_seedwork_be-0.1.8/dino_seedwork_be/storage/alchemysql/AlchemyQuerier.py
--rw-r--r--   0        0        0      210 2022-12-23 11:02:58.628158 dinohub_seedwork_be-0.1.8/dino_seedwork_be/storage/alchemysql/Repository.py
--rw-r--r--   0        0        0      163 2022-12-23 11:03:10.114696 dinohub_seedwork_be-0.1.8/dino_seedwork_be/storage/alchemysql/SerializableBase.py
--rw-r--r--   0        0        0      389 2022-12-23 07:37:41.852097 dinohub_seedwork_be-0.1.8/dino_seedwork_be/storage/alchemysql/__init__.py
--rw-r--r--   0        0        0      692 2022-12-23 11:02:20.786588 dinohub_seedwork_be-0.1.8/dino_seedwork_be/storage/alchemysql/connection.py
--rw-r--r--   0        0        0     2581 2022-12-23 11:03:24.643622 dinohub_seedwork_be-0.1.8/dino_seedwork_be/storage/alchemysql/uow.py
--rw-r--r--   0        0        0     3033 2022-12-23 11:04:31.118926 dinohub_seedwork_be-0.1.8/dino_seedwork_be/storage/uow.py
--rw-r--r--   0        0        0      635 2022-12-23 11:04:51.159797 dinohub_seedwork_be-0.1.8/dino_seedwork_be/types/ReturnType.py
--rw-r--r--   0        0        0       26 2022-12-23 11:05:01.870809 dinohub_seedwork_be-0.1.8/dino_seedwork_be/types/__init__.py
--rw-r--r--   0        0        0      407 2022-12-23 11:12:54.559790 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/__init__.py
--rw-r--r--   0        0        0      207 2022-12-23 11:06:24.172253 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/compare.py
--rw-r--r--   0        0        0      283 2022-12-23 11:06:54.771652 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/date.py
--rw-r--r--   0        0        0      615 2022-12-27 09:01:41.181769 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/dict.py
--rw-r--r--   0        0        0      676 2022-12-23 11:08:13.734593 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/faker_helpers.py
--rw-r--r--   0        0        0     7701 2022-12-23 10:42:11.168900 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/functional.py
--rw-r--r--   0        0        0     2057 2022-12-23 11:08:36.677443 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/image.py
--rw-r--r--   0        0        0      350 2022-12-23 11:08:46.041591 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/is_in_range.py
--rw-r--r--   0        0        0      147 2022-12-23 11:08:55.296254 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/list.py
--rw-r--r--   0        0        0      196 2022-12-23 11:09:12.973894 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/meta.py
--rw-r--r--   0        0        0      275 2022-12-23 11:09:38.078375 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/none_or_instance.py
--rw-r--r--   0        0        0      222 2022-12-23 11:09:49.998923 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/number.py
--rw-r--r--   0        0        0      698 2022-12-23 11:10:02.167213 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/params.py
--rw-r--r--   0        0        0       27 2022-12-23 11:05:48.492089 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/persistance/__init__.py
--rw-r--r--   0        0        0      546 2022-12-23 11:05:31.568121 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/persistance/alchemy_sql.py
--rw-r--r--   0        0        0      554 2022-12-23 11:05:59.536290 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/process/ThreadLocal.py
--rw-r--r--   0        0        0       27 2022-12-23 11:06:11.386737 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/process/__init__.py
--rw-r--r--   0        0        0     1331 2022-12-23 11:10:32.567200 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/set.py
--rw-r--r--   0        0        0      568 2022-12-23 11:10:56.528414 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/text.py
--rw-r--r--   0        0        0      825 2022-12-23 11:11:29.516372 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/validator.py
--rw-r--r--   0        0        0      196 2022-12-23 11:11:48.476854 dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/with_default_value.py
--rw-r--r--   0        0        0     1699 2022-12-27 09:16:54.531459 dinohub_seedwork_be-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2447 1970-01-01 00:00:00.000000 dinohub_seedwork_be-0.1.8/setup.py
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 dinohub_seedwork_be-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-12-16 09:09:54.053571 dinohub_seedwork_be-0.1.9/LICENSE
+-rw-r--r--   0        0        0      155 2022-12-16 09:09:54.022652 dinohub_seedwork_be-0.1.9/README.md
+-rw-r--r--   0        0        0       26 2022-12-23 11:13:56.668882 dinohub_seedwork_be-0.1.9/dino_seedwork_be/__init__.py
+-rw-r--r--   0        0        0      134 2022-12-23 10:25:34.977531 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/__init__.py
+-rw-r--r--   0        0        0       86 2022-12-23 11:14:33.893228 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/dto.py
+-rw-r--r--   0        0        0      221 2022-12-23 10:24:57.376557 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/logger.py
+-rw-r--r--   0        0        0       48 2022-12-23 06:59:49.199000 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/__init__.py
+-rw-r--r--   0        0        0      314 2022-12-27 10:05:27.400924 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/firebase/AbstractUserNotificationPushDrivingAdapter.py
+-rw-r--r--   0        0        0      876 2022-12-27 08:54:50.998107 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/firebase/FirebaseNotificationDrivingAdapter.py
+-rw-r--r--   0        0        0      108 2022-12-23 10:07:14.381257 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/firebase/__init__.py
+-rw-r--r--   0        0        0     8763 2022-12-23 10:09:15.078993 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/BrokerComponent.py
+-rw-r--r--   0        0        0     2094 2022-12-23 10:09:31.175969 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/ConnectionSettings.py
+-rw-r--r--   0        0        0     3193 2022-12-23 10:09:54.305433 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/Exchange.py
+-rw-r--r--   0        0        0     5298 2022-12-23 10:10:10.506117 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/ExchangeListener.py
+-rw-r--r--   0        0        0    10717 2022-12-23 10:10:28.653802 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/MessageConsumer.py
+-rw-r--r--   0        0        0     4147 2022-12-23 10:10:39.921907 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/MessageListener.py
+-rw-r--r--   0        0        0     1803 2022-12-23 10:10:51.188641 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/MessageParameters.py
+-rw-r--r--   0        0        0     8014 2022-12-23 10:11:07.523388 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/MessageProducer.py
+-rw-r--r--   0        0        0      116 2022-12-23 10:11:22.215423 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/MessageType.py
+-rw-r--r--   0        0        0    11445 2022-12-23 10:11:39.774950 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/Queue.py
+-rw-r--r--   0        0        0     1076 2022-12-23 10:14:04.069478 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/__init__.py
+-rw-r--r--   0        0        0      136 2022-12-23 10:09:44.676190 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/exceptions.py
+-rw-r--r--   0        0        0     9291 2022-12-23 10:14:27.944113 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/pubsub/RabbitMQPublisher.py
+-rw-r--r--   0        0        0       33 2022-12-23 10:14:38.673804 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/pubsub/__init__.py
+-rw-r--r--   0        0        0     2524 2022-12-23 10:25:11.851014 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/repository.py
+-rw-r--r--   0        0        0       21 2022-12-23 10:22:29.776198 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/rest/__init__.py
+-rw-r--r--   0        0        0       82 2022-12-23 10:15:33.452083 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/rest/fastapi/__init__.py
+-rw-r--r--   0        0        0      826 2022-12-23 10:14:58.693267 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/rest/fastapi/basic_handle_exception.py
+-rw-r--r--   0        0        0      666 2022-12-23 10:15:10.672448 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/rest/fastapi/filters.py
+-rw-r--r--   0        0        0      586 2022-12-23 10:15:22.475200 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/rest/fastapi/order.py
+-rw-r--r--   0        0        0     5861 2022-12-23 10:22:03.820241 dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/rest/utils.py
+-rw-r--r--   0        0        0     3818 2022-12-23 10:25:53.931308 dinohub_seedwork_be-0.1.9/dino_seedwork_be/application/AbstractApplicationLifeCycle.py
+-rw-r--r--   0        0        0      500 2022-12-23 10:28:40.509858 dinohub_seedwork_be-0.1.9/dino_seedwork_be/application/ApplicationLifeCycleUseCase.py
+-rw-r--r--   0        0        0      177 2022-12-23 10:29:52.819577 dinohub_seedwork_be-0.1.9/dino_seedwork_be/application/__init__.py
+-rw-r--r--   0        0        0       48 2022-12-23 10:28:51.608420 dinohub_seedwork_be-0.1.9/dino_seedwork_be/application/command.py
+-rw-r--r--   0        0        0      594 2022-12-23 10:29:01.709755 dinohub_seedwork_be-0.1.9/dino_seedwork_be/application/handler.py
+-rw-r--r--   0        0        0      313 2022-12-23 10:29:14.588549 dinohub_seedwork_be-0.1.9/dino_seedwork_be/application/query.py
+-rw-r--r--   0        0        0      463 2022-12-23 10:29:30.705966 dinohub_seedwork_be-0.1.9/dino_seedwork_be/application/service.py
+-rw-r--r--   0        0        0     1132 2022-12-23 10:30:09.907783 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/AbstractDomainEventDict.py
+-rw-r--r--   0        0        0     1246 2022-12-26 03:24:07.967231 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/AbstractIdentity.py
+-rw-r--r--   0        0        0      258 2022-12-25 16:27:09.922531 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/AggregateRoot.py
+-rw-r--r--   0        0        0     2881 2022-12-23 10:30:43.411019 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/DomainEvent.py
+-rw-r--r--   0        0        0     3327 2022-12-26 03:15:53.174620 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/DomainEventPublisher.py
+-rw-r--r--   0        0        0      414 2022-12-25 16:27:25.542484 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/DomainEventSubscriber.py
+-rw-r--r--   0        0        0      323 2022-12-23 10:31:17.425301 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/DomainService.py
+-rw-r--r--   0        0        0     1811 2022-12-23 10:31:29.392877 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/Entity.py
+-rw-r--r--   0        0        0      973 2022-12-23 10:32:18.225122 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/IdentifiedDomainObject.py
+-rw-r--r--   0        0        0      405 2022-12-23 10:32:36.045815 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/IdentifiedValueObject.py
+-rw-r--r--   0        0        0     1373 2022-12-23 10:33:04.642067 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/RegexValue.py
+-rw-r--r--   0        0        0      438 2022-12-26 04:04:58.780387 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/__init__.py
+-rw-r--r--   0        0        0     1083 2022-12-23 10:31:54.292011 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/exceptions.py
+-rw-r--r--   0        0        0      760 2022-12-23 10:32:52.407487 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/mixins.py
+-rw-r--r--   0        0        0      528 2022-12-23 10:33:17.602347 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/rules.py
+-rw-r--r--   0        0        0      244 2022-12-23 10:33:31.882913 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/utils.py
+-rw-r--r--   0        0        0      561 2022-12-23 10:36:48.237292 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/validator.py
+-rw-r--r--   0        0        0     7300 2022-12-23 10:37:52.263631 dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/value_objects.py
+-rw-r--r--   0        0        0     1002 2022-12-23 10:40:12.888448 dinohub_seedwork_be-0.1.9/dino_seedwork_be/event/EventSerializer.py
+-rw-r--r--   0        0        0      967 2022-12-23 10:40:24.388207 dinohub_seedwork_be-0.1.9/dino_seedwork_be/event/EventStore.py
+-rw-r--r--   0        0        0     2324 2022-12-23 10:41:18.136972 dinohub_seedwork_be-0.1.9/dino_seedwork_be/event/StoredEvent.py
+-rw-r--r--   0        0        0      111 2022-12-23 10:43:15.422718 dinohub_seedwork_be-0.1.9/dino_seedwork_be/event/__init__.py
+-rw-r--r--   0        0        0     3505 2022-12-23 10:41:50.025534 dinohub_seedwork_be-0.1.9/dino_seedwork_be/event/persistance/SqlAlchemyEventStore.py
+-rw-r--r--   0        0        0     3194 2022-12-23 10:42:35.569574 dinohub_seedwork_be-0.1.9/dino_seedwork_be/event/persistance/SqlAlchemyPublishedNotificationTrackerStore.py
+-rw-r--r--   0        0        0       95 2022-12-23 10:42:52.507948 dinohub_seedwork_be-0.1.9/dino_seedwork_be/event/persistance/__init__.py
+-rw-r--r--   0        0        0     2659 2022-12-23 11:13:46.604360 dinohub_seedwork_be-0.1.9/dino_seedwork_be/exceptions.py
+-rw-r--r--   0        0        0       20 2022-12-23 11:14:34.124431 dinohub_seedwork_be-0.1.9/dino_seedwork_be/fp/__init__.py
+-rw-r--r--   0        0        0      117 2022-12-23 10:43:39.692868 dinohub_seedwork_be-0.1.9/dino_seedwork_be/fp/list.py
+-rw-r--r--   0        0        0       59 2022-12-23 10:44:54.519439 dinohub_seedwork_be-0.1.9/dino_seedwork_be/logic/__init__.py
+-rw-r--r--   0        0        0    12044 2022-12-23 10:44:30.578472 dinohub_seedwork_be-0.1.9/dino_seedwork_be/logic/assertion_concern.py
+-rw-r--r--   0        0        0      455 2022-12-23 10:44:44.020251 dinohub_seedwork_be-0.1.9/dino_seedwork_be/logic/validators.py
+-rw-r--r--   0        0        0     3079 2022-12-23 10:45:15.092145 dinohub_seedwork_be-0.1.9/dino_seedwork_be/media/AbstractJsonMediaReader.py
+-rw-r--r--   0        0        0      159 2022-12-23 10:45:25.503373 dinohub_seedwork_be-0.1.9/dino_seedwork_be/media/RepresentationReader.py
+-rw-r--r--   0        0        0       75 2022-12-23 10:48:05.944147 dinohub_seedwork_be-0.1.9/dino_seedwork_be/media/__init__.py
+-rw-r--r--   0        0        0     1269 2022-12-23 10:48:26.164692 dinohub_seedwork_be-0.1.9/dino_seedwork_be/process/AbstractProcess.py
+-rw-r--r--   0        0        0     2067 2022-12-23 10:48:37.130877 dinohub_seedwork_be-0.1.9/dino_seedwork_be/process/AbstractProcessApplicationService.py
+-rw-r--r--   0        0        0      718 2022-12-23 10:48:49.228378 dinohub_seedwork_be-0.1.9/dino_seedwork_be/process/ProcessId.py
+-rw-r--r--   0        0        0     1621 2022-12-23 10:48:59.326673 dinohub_seedwork_be-0.1.9/dino_seedwork_be/process/ProcessTimeOut.py
+-rw-r--r--   0        0        0     8616 2022-12-23 10:49:08.962194 dinohub_seedwork_be-0.1.9/dino_seedwork_be/process/TimeConstrainedProcessTracker.py
+-rw-r--r--   0        0        0     1316 2022-12-23 10:49:19.029644 dinohub_seedwork_be-0.1.9/dino_seedwork_be/process/TimeConstrainedProcessTrackerRepository.py
+-rw-r--r--   0        0        0      272 2022-12-23 10:50:14.910034 dinohub_seedwork_be-0.1.9/dino_seedwork_be/process/__init__.py
+-rw-r--r--   0        0        0      783 2022-12-23 10:49:28.772379 dinohub_seedwork_be-0.1.9/dino_seedwork_be/process/timeout_event_factory.py
+-rw-r--r--   0        0        0     1129 2022-12-23 10:50:27.096845 dinohub_seedwork_be-0.1.9/dino_seedwork_be/pubsub/DefaultImplementNotificationApplicationService.py
+-rw-r--r--   0        0        0     3112 2022-12-23 10:50:42.899716 dinohub_seedwork_be-0.1.9/dino_seedwork_be/pubsub/Notification.py
+-rw-r--r--   0        0        0      886 2022-12-23 10:50:54.376921 dinohub_seedwork_be-0.1.9/dino_seedwork_be/pubsub/NotificationPublisher.py
+-rw-r--r--   0        0        0     1689 2022-12-23 10:58:52.492569 dinohub_seedwork_be-0.1.9/dino_seedwork_be/pubsub/NotificationReader.py
+-rw-r--r--   0        0        0     1173 2022-12-23 10:59:07.835347 dinohub_seedwork_be-0.1.9/dino_seedwork_be/pubsub/NotificationSerializer.py
+-rw-r--r--   0        0        0     3195 2022-12-23 10:59:20.557003 dinohub_seedwork_be-0.1.9/dino_seedwork_be/pubsub/PublishedNotificationTracker.py
+-rw-r--r--   0        0        0     1138 2022-12-23 10:59:32.477207 dinohub_seedwork_be-0.1.9/dino_seedwork_be/pubsub/PublishedNotificationTrackerStore.py
+-rw-r--r--   0        0        0      292 2022-12-23 11:00:15.454131 dinohub_seedwork_be-0.1.9/dino_seedwork_be/pubsub/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-26 04:06:29.307336 dinohub_seedwork_be-0.1.9/dino_seedwork_be/py.typed
+-rw-r--r--   0        0        0      163 2022-12-23 11:00:28.079371 dinohub_seedwork_be-0.1.9/dino_seedwork_be/serializer/AbstractSerializer.py
+-rw-r--r--   0        0        0      838 2022-12-23 11:00:39.676133 dinohub_seedwork_be-0.1.9/dino_seedwork_be/serializer/ObjectSerializer.py
+-rw-r--r--   0        0        0      365 2022-12-23 11:00:50.758546 dinohub_seedwork_be-0.1.9/dino_seedwork_be/serializer/Serializable.py
+-rw-r--r--   0        0        0       94 2022-12-23 11:01:45.872572 dinohub_seedwork_be-0.1.9/dino_seedwork_be/serializer/__init__.py
+-rw-r--r--   0        0        0       19 2022-12-23 11:03:42.645054 dinohub_seedwork_be-0.1.9/dino_seedwork_be/storage/__init__.py
+-rw-r--r--   0        0        0     5318 2022-12-27 09:07:44.119207 dinohub_seedwork_be-0.1.9/dino_seedwork_be/storage/alchemysql/AlchemyQuerier.py
+-rw-r--r--   0        0        0      210 2022-12-23 11:02:58.628158 dinohub_seedwork_be-0.1.9/dino_seedwork_be/storage/alchemysql/Repository.py
+-rw-r--r--   0        0        0      163 2022-12-23 11:03:10.114696 dinohub_seedwork_be-0.1.9/dino_seedwork_be/storage/alchemysql/SerializableBase.py
+-rw-r--r--   0        0        0      389 2022-12-23 07:37:41.852097 dinohub_seedwork_be-0.1.9/dino_seedwork_be/storage/alchemysql/__init__.py
+-rw-r--r--   0        0        0      692 2022-12-23 11:02:20.786588 dinohub_seedwork_be-0.1.9/dino_seedwork_be/storage/alchemysql/connection.py
+-rw-r--r--   0        0        0     2581 2022-12-23 11:03:24.643622 dinohub_seedwork_be-0.1.9/dino_seedwork_be/storage/alchemysql/uow.py
+-rw-r--r--   0        0        0     3033 2022-12-23 11:04:31.118926 dinohub_seedwork_be-0.1.9/dino_seedwork_be/storage/uow.py
+-rw-r--r--   0        0        0      635 2022-12-23 11:04:51.159797 dinohub_seedwork_be-0.1.9/dino_seedwork_be/types/ReturnType.py
+-rw-r--r--   0        0        0       26 2022-12-23 11:05:01.870809 dinohub_seedwork_be-0.1.9/dino_seedwork_be/types/__init__.py
+-rw-r--r--   0        0        0      407 2022-12-23 11:12:54.559790 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/__init__.py
+-rw-r--r--   0        0        0      207 2022-12-23 11:06:24.172253 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/compare.py
+-rw-r--r--   0        0        0      283 2022-12-23 11:06:54.771652 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/date.py
+-rw-r--r--   0        0        0      615 2022-12-27 09:01:41.181769 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/dict.py
+-rw-r--r--   0        0        0      676 2022-12-23 11:08:13.734593 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/faker_helpers.py
+-rw-r--r--   0        0        0     7701 2022-12-23 10:42:11.168900 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/functional.py
+-rw-r--r--   0        0        0     2057 2022-12-23 11:08:36.677443 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/image.py
+-rw-r--r--   0        0        0      350 2022-12-23 11:08:46.041591 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/is_in_range.py
+-rw-r--r--   0        0        0      147 2022-12-23 11:08:55.296254 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/list.py
+-rw-r--r--   0        0        0      196 2022-12-23 11:09:12.973894 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/meta.py
+-rw-r--r--   0        0        0      275 2022-12-23 11:09:38.078375 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/none_or_instance.py
+-rw-r--r--   0        0        0      222 2022-12-23 11:09:49.998923 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/number.py
+-rw-r--r--   0        0        0      698 2022-12-23 11:10:02.167213 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/params.py
+-rw-r--r--   0        0        0       27 2022-12-23 11:05:48.492089 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/persistance/__init__.py
+-rw-r--r--   0        0        0      557 2022-12-27 09:44:19.984295 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/persistance/alchemy_sql.py
+-rw-r--r--   0        0        0      554 2022-12-23 11:05:59.536290 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/process/ThreadLocal.py
+-rw-r--r--   0        0        0       27 2022-12-23 11:06:11.386737 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/process/__init__.py
+-rw-r--r--   0        0        0     1331 2022-12-23 11:10:32.567200 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/set.py
+-rw-r--r--   0        0        0      568 2022-12-23 11:10:56.528414 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/text.py
+-rw-r--r--   0        0        0      825 2022-12-23 11:11:29.516372 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/validator.py
+-rw-r--r--   0        0        0      196 2022-12-23 11:11:48.476854 dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/with_default_value.py
+-rw-r--r--   0        0        0     1699 2022-12-27 10:22:24.880225 dinohub_seedwork_be-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2447 1970-01-01 00:00:00.000000 dinohub_seedwork_be-0.1.9/setup.py
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 dinohub_seedwork_be-0.1.9/PKG-INFO
```

### Comparing `dinohub_seedwork_be-0.1.8/LICENSE` & `dinohub_seedwork_be-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/firebase/FirebaseNotificationDrivingAdapter.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/firebase/FirebaseNotificationDrivingAdapter.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/BrokerComponent.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/BrokerComponent.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/ConnectionSettings.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/ConnectionSettings.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/Exchange.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/Exchange.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/ExchangeListener.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/ExchangeListener.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/MessageConsumer.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/MessageConsumer.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/MessageListener.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/MessageListener.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/MessageParameters.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/MessageParameters.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/MessageProducer.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/MessageProducer.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/Queue.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/Queue.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/messaging/rabbitmq/__init__.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/messaging/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/pubsub/RabbitMQPublisher.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/pubsub/RabbitMQPublisher.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/repository.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/rest/fastapi/basic_handle_exception.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/rest/fastapi/basic_handle_exception.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/rest/fastapi/filters.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/rest/fastapi/filters.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/rest/fastapi/order.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/rest/fastapi/order.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/adapters/rest/utils.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/adapters/rest/utils.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/application/AbstractApplicationLifeCycle.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/application/AbstractApplicationLifeCycle.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/application/handler.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/application/handler.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/AbstractDomainEventDict.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/AbstractDomainEventDict.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/AbstractIdentity.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/AbstractIdentity.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/DomainEvent.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/DomainEvent.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/DomainEventPublisher.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/DomainEventPublisher.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/Entity.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/Entity.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/IdentifiedDomainObject.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/IdentifiedDomainObject.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/RegexValue.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/RegexValue.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/exceptions.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/mixins.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/mixins.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/rules.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/rules.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/validator.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/validator.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/domain/value_objects.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/domain/value_objects.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/event/EventSerializer.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/event/EventSerializer.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/event/EventStore.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/event/EventStore.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/event/StoredEvent.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/event/StoredEvent.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/event/persistance/SqlAlchemyEventStore.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/event/persistance/SqlAlchemyEventStore.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/event/persistance/SqlAlchemyPublishedNotificationTrackerStore.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/event/persistance/SqlAlchemyPublishedNotificationTrackerStore.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/exceptions.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/exceptions.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/logic/assertion_concern.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/logic/assertion_concern.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/media/AbstractJsonMediaReader.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/media/AbstractJsonMediaReader.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/process/AbstractProcess.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/process/AbstractProcess.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/process/AbstractProcessApplicationService.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/process/AbstractProcessApplicationService.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/process/ProcessId.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/process/ProcessId.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/process/ProcessTimeOut.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/process/ProcessTimeOut.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/process/TimeConstrainedProcessTracker.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/process/TimeConstrainedProcessTracker.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/process/TimeConstrainedProcessTrackerRepository.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/process/TimeConstrainedProcessTrackerRepository.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/process/timeout_event_factory.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/process/timeout_event_factory.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/pubsub/DefaultImplementNotificationApplicationService.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/pubsub/DefaultImplementNotificationApplicationService.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/pubsub/Notification.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/pubsub/Notification.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/pubsub/NotificationPublisher.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/pubsub/NotificationPublisher.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/pubsub/NotificationReader.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/pubsub/NotificationReader.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/pubsub/NotificationSerializer.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/pubsub/NotificationSerializer.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/pubsub/PublishedNotificationTracker.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/pubsub/PublishedNotificationTracker.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/pubsub/PublishedNotificationTrackerStore.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/pubsub/PublishedNotificationTrackerStore.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/serializer/ObjectSerializer.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/serializer/ObjectSerializer.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/storage/alchemysql/AlchemyQuerier.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/storage/alchemysql/AlchemyQuerier.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/storage/alchemysql/connection.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/storage/alchemysql/connection.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/storage/alchemysql/uow.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/storage/alchemysql/uow.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/storage/uow.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/storage/uow.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/types/ReturnType.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/types/ReturnType.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/dict.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/dict.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/faker_helpers.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/faker_helpers.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/functional.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/functional.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/image.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/image.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/params.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/params.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/persistance/alchemy_sql.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/persistance/alchemy_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, List
 
-from dino_seedwork_be.adapters import Repository
+from dino_seedwork_be.adapters.repository import Repository
 
 __all__ = [
     "alchemy_execute_query_on_repository",
     "tuple_row_to_dict",
     "tuple_rows_to_dict",
 ]
```

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/process/ThreadLocal.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/process/ThreadLocal.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/set.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/set.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/text.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/text.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/dino_seedwork_be/utils/validator.py` & `dinohub_seedwork_be-0.1.9/dino_seedwork_be/utils/validator.py`

 * *Files identical despite different names*

### Comparing `dinohub_seedwork_be-0.1.8/pyproject.toml` & `dinohub_seedwork_be-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project.urls]
 "Homepage" = "https://github.com/pypa/sampleproject"
 "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
 
 [tool.poetry]
 name = "dinohub-seedwork-be"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   "Tuan Cau Rao <tuan.pt@orai.io>",
 ]
 description = "A seedwork for DinoHub service"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `dinohub_seedwork_be-0.1.8/setup.py` & `dinohub_seedwork_be-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
  'sqlalchemy-utils>=0.38.3,<0.39.0',
  'toolz>=0.11.2,<0.12.0',
  'uvicorn[standard]>=0.17.6,<0.18.0',
  'validators>=0.19.0,<0.20.0']
 
 setup_kwargs = {
     'name': 'dinohub-seedwork-be',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'A seedwork for DinoHub service',
     'long_description': '# DINO hub seedwork\n\nThis is a package contains\n  * DDD (Domain Driven Design) artifact\n  * Functional programming with Returns\n  * Basic helpers function\n',
     'author': 'Tuan Cau Rao',
     'author_email': 'tuan.pt@orai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dinohub_seedwork_be-0.1.8/PKG-INFO` & `dinohub_seedwork_be-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dinohub-seedwork-be
-Version: 0.1.8
+Version: 0.1.9
 Summary: A seedwork for DinoHub service
 Author: Tuan Cau Rao
 Author-email: tuan.pt@orai.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

