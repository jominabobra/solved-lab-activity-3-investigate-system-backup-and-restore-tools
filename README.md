Download Link: https://assignmentchef.com/product/solved-lab-activity-3-investigate-system-backup-and-restore-tools
<br>
Purpose: Assess and Document Tools to Backup and Restore the System Hard Drive for a Windows 8.1 Workstation.

<ol>

 <li>Assess and document the use of a system backup tool or disk imaging utility to create a “known-good” copy of the system hard drive for a Windows 8.1 Workstation.</li>

 <li>Assess and document the use of “known-good” copies of system hard drives to restore system availability after an incident.</li>

</ol>

Overview:

For this activity, we will focus upon assessing and documenting tools which are used in the <strong>preparation phase</strong> and in the <strong>containment, eradication, and recovery phase</strong> of the Incident Response Process (as defined in NIST SP 800-61r2). These tools will support incident responders by providing “access to images of clean OS and application installations for restoration and recovery purposes” (Cichonski, Millar, Grance, &amp; Scarfone, 2012, p. 23).

Situation Report:

Recent contracts with the Departments of Defense and Homeland Security have imposed additional security requirements upon the company and its SCADA lab operations. The company is now required to comply with NIST Special Publication 800-171 <em>Protecting Controlled Unclassified Information in Nonfederal Information Systems and Organizations. </em>The company must also comply with provisions of the Defense Federal Acquisition Regulations (DFARS) including section 252-204-7012 <em>Safeguarding Covered Defense Information and Cyber Incident Reporting.</em> These requirements are designed to ensure that sensitive technical information, provided by the federal government and stored on computer systems in the Sifers-Grayson SCADA lab, is protected from unauthorized disclosure. This information includes software designs and source code for Industrial Control Systems for which Sifers-Grayson is providing software support and maintenance. The contract requirements also mandate that Sifers-Grayson report cyber incidents to the federal government in a timely manner.

The engineering and design workstations in the Sifers-Grayson SCADA Lab were upgraded from Windows XP to Windows 8.1 professional three years ago after the lab was hit with a ransomware attack that exploited several Windows XP vulnerabilities. A second successful ransomware attack occurred three months ago. The company paid the ransom in both cases because the lab did not have file backups that it could use to recover the damaged files (in the first case) and did not have system backups that it could use to rebuild the system hard drives (in the second case).

The SCADA Lab is locked into using Windows 8.1. The planned transition to Windows 10 is on indefinite hold due to technical problems encountered during previous attempts to modify required software applications to work under the new version of the operating system. This means that an incident response and recovery capability for the lab must support the Windows 8.1 operating system and the related engineering software applications. <strong>But, the customer’s technical representatives have strongly suggested that Sifers-Grayson personnel use backup utilities that are not specific to the Windows 8.1 operating system.  </strong>

<strong>Reference</strong>

Cichonski, P., Millar, T., Grance, T., &amp; Scarfone, K. (2012). <em>Computer security incident handling guide </em>(NIST SP 800-62 rev. 2). http://dx.doi.org/10.6028/NIST.SP.800-61r2

Solved

Prepare draft incident response guidance to be included in the Sifers-Grayson <em>Incident Responder’s Handbook</em>. Your draft guidance will explain the use of a commercially available system hard drive backup tool. Your guidance will explain how to use your selected third-party tool to create either a system backup or a system image (bit for bit copy) of the system hard drive for a Windows 8.1 workstation. Suggested tools include: Acronis, FTK Imager, and Paladin.

You will create two separate procedures. The first will explain how to perform a backup. The second will explain how to use the known-good backup to restore the system hard drive (also, how to restore to a new hard drive). Both procedures must address the use of cryptographic hash codes (e.g. MD5 or SHA-256) to verify the integrity of the backup files and/or system image files.

<h2>Instructions</h2>

<h3>Part (a): Creating a “Known-Good” (Clean) Disk Image for a Windows 8.1 Workstation</h3>

<ol>

 <li>Using the Internet, research commercially available system backup tool or application. (Do not use any features or utilities that are part of the Windows operating system.) Then, identify appropriate sources of information and instructions for your selected tool. Using those sources, research the procedures required to

  <ol start="8">

   <li>Create a “known good” copy (system backup or complete system image) of the hard drive containing the Windows 8.1 system and installed applications for a workstation in the SCADA lab.</li>

   <li>Generate a hash code for use in verifying the validity and integrity of the backup file or system image file. (If your backup utility does not provide this, you will need to find a separate tool that will generate an MD-5 or SHA-256 hash value for the image file or backup file. See <a href="https://www.howtogeek.com/67241/htg-explains-what-are-md5-sha-1-hashes-and-how-do-i-check-them/">https://www.howtogeek.com/67241/htg-explains-what-are-md5-sha-1-hashes-and-how-do-i-check-them/</a> for an explanation of file integrity checking using hash codes.)</li>

   <li>You should also research and document best practices for labeling and storing the digital media containing the backup files and/or system image files. The storage location should provide secure storage yet be readily available to incident responders in the event of an incident. The label or storage log should include the hash value for each backup file and system image file.</li>

  </ol></li>

 <li>Identify how the backup tool could be used during the <strong>preparation phase</strong> of the incident response and recovery process. Typical uses include:

  <ol>

   <li>Create a “known good” backup that contains a complete, verified and approved system configuration that includes the operating system and all required application software.</li>

   <li>Create a copy of the original operating system installation (before software applications are installed).</li>

  </ol></li>

 <li>Write a <em>guidance document </em>that identifies the tool, explains the capabilities it provides, and then lists and briefly describes the recommended uses identified under item #2. Add a list of resources that can be consulted for additional information. Next, summarize the procedures required to perform the tasks listed under item #1 (do not provide step-by-step instructions). Close your guidance document with a Notes / Warnings / Restrictions section that answers the question “Is there anything else the incident responder needs to be aware of when using this tool?”</li>

</ol>




<h3>Part (b): Using a “Known-Good” (Clean) Disk Image to Restore the System Hard Drive for a Windows 8.1 Workstation</h3>

<ol>

 <li>Use the same tool and tool research as performed for part (a) of this lab. If necessary, identify additional sources of information and instructions for using your selected tool(s) to perform the following tasks:

  <ol>

   <li>Verify the validity of the backup image or file (using the hash code).</li>

   <li>Use the “known good” copy (system backup or system image) to rebuild a workstation hard drive so that it contains the Windows 8.1 operation system and installed applications.</li>

  </ol></li>

 <li>Identify how the tool could be used during the <strong>containment, eradication &amp; recovery phase</strong> of the incident response and recovery process. Typical uses include:

  <ol>

   <li>Restore workstation hard drives to a “known good” configuration.</li>

   <li>Build a new system disk using a replacement or newly purchased hard drive.</li>

   <li>Restore the system to full operating status after an attack or suspected attack.</li>

  </ol></li>

 <li>Write a <em>guidance document </em>that identifies the tool, explains the capabilities it provides, and then lists and briefly describes the recommended uses identified under item #2. Add a list of resources that can be consulted for additional information. Next, summarize the procedures required to perform the tasks listed under item #1 (do not provide step-by-step instructions). Close your guidance document with a Notes / Warnings / Restrictions section that answers the question “Is there anything else the incident responder needs to be aware of when using this tool?”</li>

</ol>

<h3>Finalize Your Deliverable</h3>

<ol>

 <li>Using the grading rubric as a guide, refine your incident response guidance. Your final products should be suitable for inclusion in the organization’s <em>Incident Responder’s Handbook</em>. Remember that you are preparing multiple guidance documents, which must be presented separately.</li>

 <li>As appropriate, cite your sources using footnotes or another appropriate citation style.</li>

 <li>Use the <em>resources </em>section to provide information about recommended readings and any sources that you cite. Use a standard bibliographic format (you may wish to use APA since this is required in other CSIA courses). Information about sources and recommended readings, including in-text citations, should be formatted consistently and professionally.</li>

 <li>Your submission file for this assignment should start with a title page which lists the following information:</li>

</ol>

<ul>

 <li>Lab Title and Number</li>

 <li>Date</li>

 <li>Your Name</li>

</ul>

<ol start="5">

 <li>The <strong>CSIA 310 Template for Lab Deliverable.docx</strong> file is set up to provide the required title page and two <em>incident response guidance</em> Use the first template for your “How to Backup” guidance. Use the second procedure template for your “How to Restore” guidance.</li>

</ol>





