# codex-gui maintenance branch

The `codex-gui` branch carries the TextView changes used by
[`Open-Agents-GUI/codex-gui`](https://github.com/Open-Agents-GUI/codex-gui).

It starts from upstream commit
`972a3ebfd01afca7da6d8b6f31c9a51288ea5565`. The downstream changes are kept
as commits on top of that upstream history so future updates can be performed
with a regular merge or rebase instead of copying a source snapshot.

The customizations are intentionally concentrated in `crates/ui/src/text` and
the scrollable mask. They provide incremental Markdown parsing and layout,
stable virtual-list scrolling during streaming updates, transcript custom
blocks and selection, append fades, and codex-gui's trailing overscroll
behavior.

The branch is consumed by an exact Git revision. Update that revision in
codex-gui only after the branch has been checked against the matching GPUI
revision.
