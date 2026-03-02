# TestFlight Smoke Checklist (v1.2)

Use this checklist after uploading the build to TestFlight and before App Review submission.

## Build and Distribution

- [ ] Build archive succeeds in Xcode Organizer.
- [ ] Build uploads to App Store Connect without validation errors.
- [ ] Build finishes TestFlight processing.
- [ ] Internal testers can install the build.

## Device Matrix

- [ ] Test on at least 2 physical iPhones.
- [ ] Both devices signed into the same Apple ID for iCloud sync validation.
- [ ] At least one device has camera hardware that supports barcode scanning.

## Cloud Sync

- [ ] Device A adds 3+ products; Device B receives them.
- [ ] Device A edits quantity/date/location; Device B reflects updates.
- [ ] Device A deletes an item; Device B reflects deletion.
- [ ] Barcode memory sync check: scan/manual-save on A, confirm lookup autofill behavior on B.
- [ ] If iCloud is unavailable, app still launches and Settings shows local fallback state.

## Scanner and Permissions

- [ ] First scanner launch shows camera permission prompt with correct usage text.
- [ ] Denied camera permission path shows recovery CTA to Settings.
- [ ] Successful scan path works (lookup -> confirm -> save).
- [ ] Manual fallback path works when barcode not found.

## Subscription and Gating

- [ ] Paywall displays monthly price and legal links.
- [ ] Purchase succeeds for test account.
- [ ] Restore purchases succeeds after reinstall/relaunch.
- [ ] Free-tier gating still limits to 5 items.
- [ ] Pro unlock removes item/feature limits.

## Notifications

- [ ] Notification permission request appears.
- [ ] Lead-time settings (1/3/7) save correctly.
- [ ] Notification time setting saves correctly.
- [ ] Scheduled reminders appear for sample products.

## App Store Submission Readiness

- [ ] App metadata copy matches actual behavior (subscription + iCloud sync wording).
- [ ] Support URL is reachable.
- [ ] Privacy Policy URL is reachable.
- [ ] Latest screenshots are uploaded to matching device slots.
- [ ] Release notes updated for this version.

## Sign-off

- [ ] No P0/P1 issues open.
- [ ] Build marked “Ready for Review”.
