This repo contains some results from running FIO on 4 of Micron P320h PCIe SSD 2.5" form factor drives that were delivered with Dell PowerEdge 720.
NB: these are obviously NOT NVMe based SSDs, but use some proprietary Micron drivers (mtip32xx).
Find more details at StorageReview: http://www.storagereview.com/micron_p320h_25_pcie_application_accelerator_review 
  
Example of such a fio run:
#time fio rsscd_ssd-steadystate.fio --output=rssdd-steady-state_2.log

**BEWARE** these runs will **DESTROY ALL DATA** on your disks since the preconditioning is done by randomly writing over the drives in 3 loops!

