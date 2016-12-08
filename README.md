# Clean kubernetes

This repo just contains scripts for purging a local k8s repo

Usage:

    # Delete all kubernetes jobs, services, etc (related to pachyderm) without killing
    # hyperkube and turning down the k8s cluster itsef:
    $ reset_kube

    # Delete all k8s jobs, services, etc (related to pachyderm) and kill hyperkube
    # so you can restart it (for e.g. upgrades or flag flips)
    $ reset_kube --hard
