worker: env DB_POOL=20 LIBRATO_AUTORUN=1 bundle exec sidekiq -c 20 -q critical,3 -q feed_refresher_receiver,2 -q default -q image
worker_slow: env DB_POOL=2 bundle exec sidekiq -c 2 -q worker_slow_critical,2 -q worker_slow,1
clock: bundle exec clockwork lib/clock.rb
