The SCSI standard
	Small Computer Systems Interface
	not really "small" any longer

	originally designed to string many peripherals together into a single cable/ controller
		up to 16 devices in a SCSI "chain"
	
	many different formats
		fast SCSI, Ultra SCSI, Ultra Wide SCSI, Ultra2 SCSI, ultra3 	SCSI, Ultra-320 SCSI, Ultra-640 SCSI, iSCSI (SCSI over IP)

SCSI advantages
	not just for hard drives
		scanners, tape drives, CD-ROM drives
	Many  devices on a single bus
		8 on narrow bus, 16 on wide bus
	very intelligent interface functionality
		much of the difficult configuration work is done between the SCSI devices
		
	Industry Longevity
		well supported in the enterprise
		A standard drive for virtual systems

SCSI ID and logical unit (LUN)
	every SCSI device on a single bus is assigned a separate ID number
		SCSI id 0 (SCSI controller), ID 2 (hard drive), ID 3 (CD-ROM)
	logical unit (LUNs) are defined within each SCSI ID
		separate drives in a storage array or virtual machine
	the signal at the "end" of physical SCSI  bus is terminated
		can  be internal to the device or a separate termination device
	serial attached SCSI (SAS) devices have no jumper, terminators, or settings
	
	
serial attached SCSI 
	move from parallel to serial
		increased throughput
		similar to the move from PATA to SATA
	point-to-point
		no more daisy chains
	no termination required
		the bus has two devices on it
	the control and management of SCSI  
		the speed of a serial connection