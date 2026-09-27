# Bootstrap is vendored, not built, under assets/ so Jekyll publishes it:
# `rake 'bootstrap:status[, assets]'` compares it to upstream, and
# `rake 'bootstrap:update[, assets]'` refreshes it to the version in
# assets/.bootstrap-version. Every task takes the `assets` path, since that is
# where the version file and vendor/ live.
# See https://github.com/xoengineering/bootstrap-vendor.
require "bootstrap/vendor"
load "tasks/bootstrap.rake"
