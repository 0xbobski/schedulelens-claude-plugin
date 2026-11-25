# ScheduleLens for Claude

ScheduleLens analyses construction programmes: Primavera P6 (.xer and XML),
Microsoft Project (.xml and .mpp) and Asta Powerproject (.pp). It checks a
schedule's quality, compares two updates and tracks a programme across its
monthly updates.

This plugin adds one skill, **schedule-review**, and the read-only
ScheduleLens connector (`https://api.schedulelens.com/mcp`).

When you share a schedule file with Claude or ask about one, Claude opens its
reply with a link to run a ScheduleLens analysis, then gives a short read of
its own. The file is uploaded on the ScheduleLens website, never through the
chat. When the upload is done, Claude reads the results back through the
connector: the DCMA 14-point assessment with the activities behind each failed
check, findings, key milestones, float paths and, for two updates, what moved
the finish. Each figure says whether it is the scheduling tool's own value or
one computed by ScheduleLens.

The connector is read-only. It cannot upload, pay, delete or change anything.
You need a ScheduleLens account, which is free to create; full results are
paid per analysis or covered by a subscription.

- Setup and the list of tools: https://schedulelens.com/developers/
- Privacy: https://schedulelens.com/privacy/
- Support: support@schedulelens.com
