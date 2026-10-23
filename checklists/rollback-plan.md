# Rollback Plan
Owner: on-call release manager, who must be reachable before any production push.

1. Freeze the release and announce the rollback in the incident channel.
2. Confirm the last known-good version tag with the release manager.
3. Re-deploy the last known-good build to production using the standard pipeline.
4. Verify the metrics dashboard shows the previous, healthy baseline.
5. Notify customer-facing teams so comms can be updated or withdrawn.
6. Capture a timeline of what failed and file a follow-up issue.
7. Run the post-rollback review before scheduling the next attempt.
