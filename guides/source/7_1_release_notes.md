**DO NOT READ THIS FILE ON GITHUB, GUIDES ARE PUBLISHED ON https://guides.rubyonrails.org.**

Ruby on Rails 7.1 Release Notes
===============================

Highlights in Rails 7.1:

--------------------------------------------------------------------------------

Upgrading to Rails 7.1
----------------------

If you're upgrading an existing application, it's a great idea to have good test
coverage before going in. You should also first upgrade to Rails 7.0 in case you
haven't and make sure your application still runs as expected before attempting
an update to Rails 7.1. A list of things to watch out for when upgrading is
available in the
[Upgrading Ruby on Rails](upgrading_ruby_on_rails.html#upgrading-from-rails-7-0-to-rails-7-1)
guide.

Major Features
--------------

Railties
--------

Please refer to the [Changelog][railties] for detailed changes.

### Removals

### Deprecations

### Notable changes

Action Cable
------------

Please refer to the [Changelog][action-cable] for detailed changes.

### Removals

### Deprecations

### Notable changes

Action Pack
-----------

Please refer to the [Changelog][action-pack] for detailed changes.

### Removals

*   Remove deprecated behavior on `Request#content_type`

*   Remove deprecated ability to assign a single value to `config.action_dispatch.trusted_proxies`.

*   Remove deprecated `poltergeist` and `webkit` (capybara-webkit) driver registration for system testing.

### Deprecations

*   Deprecate `config.action_dispatch.return_only_request_media_type_on_content_type`.

*   Deprecate `AbstractController::Helpers::MissingHelperError`

*   Deprecate `ActionDispatch::IllegalStateError`.

### Notable changes

Action View
-----------

Please refer to the [Changelog][action-view] for detailed changes.

### Removals

*   Remove deprecated constant `ActionView::Path`.

*   Remove deprecated support to passing instance variables as locals to partials.

### Deprecations

### Notable changes

Action Mailer
-------------

Please refer to the [Changelog][action-mailer] for detailed changes.

### Removals

### Deprecations

### Notable changes

Active Record
-------------

Please refer to the [Changelog][active-record] for detailed changes.

### Removals

*   Remove support for `ActiveRecord.legacy_connection_handling`.

*   Remove deprecated `ActiveRecord::Base` config accessors

* Remove support for `:include_replicas` on `configs_for`. Use `:include_hidden` instead.

*   Remove deprecated `config.active_record.partial_writes`.

*   Remove deprecated `Tasks::DatabaseTasks.schema_file_type`.

### Deprecations

### Notable changes

Active Storage
--------------

Please refer to the [Changelog][active-storage] for detailed changes.

### Removals

*   Remove deprecated invalid default content types in Active Storage configurations.

*   Remove deprecated `ActiveStorage::Current#host` and `ActiveStorage::Current#host=` methods.

*   Remove deprecated behavior when assigning to a collection of attachments. Instead of appending to the collection,
    the collection is now replaced.

*   Remove deprecated `purge` and `purge_later` methods from the attachments association.

### Deprecations

### Notable changes

Active Model
------------

Please refer to the [Changelog][active-model] for detailed changes.

### Removals

### Deprecations

### Notable changes

Active Support
--------------

Please refer to the [Changelog][active-support] for detailed changes.

### Removals

*   Remove deprecated override of `Enumerable#sum`.

*   Remove deprecated `ActiveSupport::PerThreadRegistry`.

*   Remove deprecated option to passing a format to `#to_s` in `Array`, `Range`, `Date`, `DateTime`, `Time`,
    `BigDecimal`, `Float` and, `Integer`.

*   Remove deprecated override of `ActiveSupport::TimeWithZone.name`.

*   Remove deprecated `active_support/core_ext/uri` file.

*   Remove deprecated `active_support/core_ext/range/include_time_with_zone` file.

*   Remove implicit conversion of objects into `String` by `ActiveSupport::SafeBuffer`.

*   Remove deprecated `ActiveSupport::Notifications::Event#children` and  `ActiveSupport::Notifications::Event#parent_of?`.

*   Remove deprecated support to generate incorrect RFC 4122 UUIDs when providing a namespace ID that is not one of the
    constants defined on `Digest::UUID`.

### Deprecations

*   Deprecate `config.active_support.disable_to_s_conversion`.

*   Deprecate `config.active_support.remove_deprecated_time_with_zone_name`.

*   Deprecate `config.active_support.use_rfc4122_namespaced_uuids`.

### Notable changes

Active Job
----------

Please refer to the [Changelog][active-job] for detailed changes.

### Removals

### Deprecations

### Notable changes

Action Text
----------

Please refer to the [Changelog][action-text] for detailed changes.

### Removals

### Deprecations

### Notable changes

Action Mailbox
----------

Please refer to the [Changelog][action-mailbox] for detailed changes.

### Removals

### Deprecations

### Notable changes

Ruby on Rails Guides
--------------------

Please refer to the [Changelog][guides] for detailed changes.

### Notable changes

Credits
-------

See the
[full list of contributors to Rails](https://contributors.rubyonrails.org/)
for the many people who spent many hours making Rails, the stable and robust
framework it is. Kudos to all of them.

[railties]:       https://github.com/rails/rails/blob/main/railties/CHANGELOG.md
[action-pack]:    https://github.com/rails/rails/blob/main/actionpack/CHANGELOG.md
[action-view]:    https://github.com/rails/rails/blob/main/actionview/CHANGELOG.md
[action-mailer]:  https://github.com/rails/rails/blob/main/actionmailer/CHANGELOG.md
[action-cable]:   https://github.com/rails/rails/blob/main/actioncable/CHANGELOG.md
[active-record]:  https://github.com/rails/rails/blob/main/activerecord/CHANGELOG.md
[active-storage]: https://github.com/rails/rails/blob/main/activestorage/CHANGELOG.md
[active-model]:   https://github.com/rails/rails/blob/main/activemodel/CHANGELOG.md
[active-support]: https://github.com/rails/rails/blob/main/activesupport/CHANGELOG.md
[active-job]:     https://github.com/rails/rails/blob/main/activejob/CHANGELOG.md
[action-text]:    https://github.com/rails/rails/blob/main/actiontext/CHANGELOG.md
[action-mailbox]: https://github.com/rails/rails/blob/main/actionmailbox/CHANGELOG.md
[guides]:         https://github.com/rails/rails/blob/main/guides/CHANGELOG.md
