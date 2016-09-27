# LINUX_RT_PLUS

This is Archlinux' standard Linux-rt package in AUR, plus additional patchwork and features;

# Nvidia fix on -rt kernels: 

fix-race-in-PRT-wait-for-completion-simple-wait-code_Nvidia-RT-160319.patch

# dcache fixup for performance regression

* 0001-fix-dcache-try-1.patch

# BFQ io Scheduler

* 0001-block-cgroups-kconfig-build-bits-for-BFQ-v7r11-4.6.0.patch
* 0001-linux-4.6-rtlwifi-fix-atomic.patch
* 0002-block-introduce-the-BFQ-v7r11-I-O-sched-for-4.6.0.patch
* 0003-block-bfq-add-Early-Queue-Merge-EQM-to-BFQ-v7r11-for.patch
* 0004-block-bfq-turn-BFQ-v7r11-for-4.6.0-into-BFQ-v8r3-for.patch

# Additional cpu optimizations for gcc

* enable_additional_cpu_optimizations_for_gcc_v4.9+_kernel_v3.15+.patch.gz

# Selected Clear Linux Patchwork;

* 0109-intel_idle-tweak-cpuidle-cstates.patch
* 0111-init_task-faster-timerslack.patch
* 0113-fs-ext4-fsync-optimize-double-fsync-a-bunch.patch
* 0114-overload-on-wakeup.patch
* 0115-bootstats-add-printk-s-to-measure-boot-time-in-more-.patch
* 0116-fix-initcall-timestamps.patch
* 0117-smpboot-reuse-timer-calibration.patch
* 0119-Initialize-ata-before-graphics.patch
* 0120-reduce-e1000e-boot-time-by-tightening-sleep-ranges.patch
* 0124-give-rdrand-some-credit.patch

The 'overload-on-lwakeup.patch' addresses the 'wastedcores' paper/research found here; source https://github.com/jplozi/wastedcores ... Most of the rest of these (Clear linux) patches are just 'testers', but I haven't noticed any perfromance regressions or bugs when making use of them, thus far.
