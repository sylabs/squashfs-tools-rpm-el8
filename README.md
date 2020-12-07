# squashfs-tools EL 8 RPM Packaging

This is the upstream EL8 squashfs-tools 4.3-19.el8 patched with:

https://github.com/plougher/squashfs-tools/commit/de03266983ceb62e5365aac84fcd3b2fd4d16e6f

To fix:

https://bugzilla.redhat.com/show_bug.cgi?id=1785652

It is needed to avoid sporadic rare failures of `mksquashfs` in Singularity testing on large multi-core machines where a very large number of `mksquashfs` runs take place during `make e2e-test`.

