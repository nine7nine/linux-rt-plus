# LINUX_RT_PLUS

This is Archlinux' standard Linux-rt package in AUR, plus additional patchwork and features;

# BFQ io Scheduler
* 0001-block-cgroups-kconfig-build-bits-for-BFQ-v7r11-4.6.0.patch
* 0002-block-introduce-the-BFQ-v7r11-I-O-sched-for-4.6.0.patch
* 0003-block-bfq-add-Early-Queue-Merge-EQM-to-BFQ-v7r11-for.patch
* 0004-block-bfq-turn-BFQ-v7r11-for-4.6.0-into-BFQ-v8r3-for.patch

Paolo's excellent BFQ io scheduler. 

More info; http://algo.ing.unimo.it/people/paolo/disk_sched/

# UKSM (Ultra Kernel Samepage Merging)
* uksm-0.1.2.5-for-v4.6.patch

Uksm, very handy for VMs or processes where memory can be saved by de-duplicating it. 

More info; http://kerneldedup.org/en/projects/uksm/introduction/

# Additional cpu optimizations for gcc
* enable_additional_cpu_optimizations_for_gcc_v4.9+_kernel_v3.15+.patch.gz

Graysky's wonderful kernel_gcc_patch.

More info; https://github.com/graysky2/kernel_gcc_patch

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

Clear Linux, built by Intel; a distribution built for the cloud.

More Info; https://clearlinux.org/

source package/srpm; https://download.clearlinux.org/current/source/SRPMS/linux-4.7.4-262.src.rpm

The 'overload-on-lwakeup.patch' addresses the 'wastedcores' problem / research paper on linux 4.0+    

More Info, source: https://github.com/jplozi/wastedcores 

the rest of these Clear Linux patches are 'testers', thus far.
