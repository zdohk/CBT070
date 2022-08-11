~~~~~~~~~~~~~~~~

//***FILE 070 SEVERAL MVS MODIFICATIONS IN SMP FORMAT THAT          *   FILE 070
//*           HAVE BEEN RECEIVED FROM COMPUTER SCIENCES CORP.       *   FILE 070
//*           SAN DIEGO, CALIFORNIA 92123.  AS WITH EVERYTHING      *   FILE 070
//*           ON THIS TAPE USE AT YOUR OWN RISK.                    *   FILE 070
//*                                                                 *   FILE 070
//*           CURRENT ADDRESS FOR INQUIRIES:                        *   FILE 070
//*                                                                 *   FILE 070
//*               C.M. SINGER                                       *   FILE 070
//*               COMPUTER SCIENCES CORPORATION - TMD               *   FILE 070
//*               MAIL ZONE W1-5311                                 *   FILE 070
//*               5021 KEARNY VILLA ROAD                            *   FILE 070
//*               SAN DIEGO, CALIFORNIA 92123-1407                  *   FILE 070
//*                                                                 *   FILE 070
//*               TELEPHONE 619-573-3020                            *   FILE 070
//*                                                                 *   FILE 070
//*           THE FOLLOWING IS A LIST OF THE MODIFICATIONS FROM     *   FILE 070
//*           GENERAL DYNAMICS THAT ARE INCLUDED IN THIS FILE.      *   FILE 070
//*           NOTE !.  CODE THAT IS PROPRIETARY OR COPYRIGHTED IS   *   FILE 070
//*           NOT INCLUDED EVEN THOUGH THE FOLLOWING LIST MAY IMPLY *   FILE 070
//*           THAT IT IS.                                           *   FILE 070
//*                                                                 *   FILE 070
//*             ALLOW DF/DSS TO RESTORE TO ALLOC VOL                *   FILE 070
//*             DF/DSS ENQ EXIT - SKIP ENQ FOR ALL VOLS             *   FILE 070
//*             FORCE DF/DSS TO RESTORE DSN LIKE FDRDSF             *   FILE 070
//*             UPDATE GDG BASE LEVEL AT STEP END                   *   FILE 070
//*             MAKE '#' TAB CHARACTER FOR TSO EDIT                 *   FILE 070
//*             CHANGE VARY ON MOUNT ATTRIB TO PRIVATE              *   FILE 070
//*             DO NOT ALLOW VIO FOR LARGE DATASETS, ETC.           *   FILE 070
//*             IMS/VS AND NETEX RESOURCE CLEANUP MOD               *   FILE 070
//*             IGC0805A ZAP FOR IMSVS FORMATTED DUMPS              *   FILE 070
//*             IEFU83 TO NOT WRITE CERTAIN RECORDS, ETC            *   FILE 070
//*             MAKE DEFAULT TSO ALLOC DISP=SHR                     *   FILE 070
//*             BYPASS 'DATA SET NOT FREED MESSAGE'                 *   FILE 070
//*             REGION LIMIT VALUES                                 *   FILE 070
//*             EXTEND CERTAIN TSO USERS WAIT TIME TO 5 HR          *   FILE 070
//*             LIMIT NUMBER OF RECORDS FOR SYS1.BROADCAST          *   FILE 070
//*             LOGON PARAMTER CSECT                                *   FILE 070
//*             INSTALL STEP END STATISTICS MODULE                  *   FILE 070
//*             MAKE REAL DASD NOT IN VATLST PRIV/RSVD              *   FILE 070
//*             MAKE 'RETAIN' DEFAULT VOL SPECIFICATION             *   FILE 070
//*             USE IEASYSXX AS DEFAULT (XX=F(CPU SERIAL))          *   FILE 070
//*             TSO SUBMIT EXIT - KILL BAD JOBNAMES                 *   FILE 070
//*             CHANGES TO HOT IO DETECTION CONSTANTS               *   FILE 070
//*             SUPPLY OUR IEAVMXIT (CHANGE ROUTE CODES)            *   FILE 070
//*             ADD X AS SUBCOMMAND OF EDIT                         *   FILE 070
//*             PUT ACCT NUMBER IN ACF2 ACCT FIELD                  *   FILE 070
//*             DECREASE GVTOLINT AND GVTMEINT                      *   FILE 070
//*             INCREASE NIP SQA ALLOCATION                         *   FILE 070
//*             SMF EXIT TO CATCH TYPE04 & 34 RECORDS               *   FILE 070
//*             ZAP DYNALLOC TO SYSDA FROM SYSALLDA                 *   FILE 070
//*             ZAP EXTERNAL WTR FOR JESLOGX (AJSW040)              *   FILE 070
//*             UPDATE MACRO FOR SYSOUT COST EST.(AJSW042)          *   FILE 070
//*             INCREASE NUMBER OF DEVICES ALLOWED TO 512           *   FILE 070
//*             INTERACTIVE DATA TRANSMISSION OPTIONS DSECT         *   FILE 070
//*             ACF2 PRE-VALIDATION EXIT                            *   FILE 070
//*             ACF2 VIOLATION EXIT                                 *   FILE 070
//*             ACF2 LOGON POST VALIDATION EXIT                     *   FILE 070
//*             COMMAND LIMITING LIST FOR ACF2                      *   FILE 070
//*             ACF2/IMS INSTALLATION OPTIONS PROD & TEST           *   FILE 070
//*             ACF2 FDR RECORD DEFINITION                          *   FILE 070
//*             SKIP SECURITY CHECK FOR TAPES OUTSIDE TMS           *   FILE 070
//*             ADD INFO TO TYPE 26 SMF RECORD                      *   FILE 070
//*             SET TRANSMISSION SEQUENCE FOR NJE SECTIONS          *   FILE 070
//*             INSTALL NOTE11 NEXT-KEY FUNCTION                    *   FILE 070
//*             NOTE12 INSTALLATION UM12001                         *   FILE 070
//*             MAKE OLDGENER ALIAS                                 *   FILE 070
//*             ALLOW ISAM UPDATES WITH DISP=SHR                    *   FILE 070
//*             IF DATASET IS VIO THEN BUFNO=1                      *   FILE 070
//*             PUT CHARGE NUMBER IN FMT1 DSCB                      *   FILE 070
//*             DF/DS DASD ALLOCATION PREPROCESSING EXIT            *   FILE 070
//*             DF/DS DASD ALLOCATION POSTPROCESSING EXIT           *   FILE 070
//*             CHANGES TO SYSGEN JOBCARD MACRO                     *   FILE 070
//*             SPF COMMAND TO FRONT END ISPF/PDF                   *   FILE 070
//*             TSO COMMAND IN ISPF COMMAND TABLE                   *   FILE 070
//*             MIGRATION VOLUME EXIT                               *   FILE 070
//*             HSM TAPE DATASET EXIT                               *   FILE 070
//*             HSM - ACF2 INTERFACE EXIT                           *   FILE 070
//*             HSM MIGRATION EXIT - LIMIT TO < 50 CYL.             *   FILE 070
//*             ACF2,RINGCHK,EXPDTCHK,STARS FOR IMS,CICS            *   FILE 070
//*             ACCT + MAKE LINES FOR STC + TSO = OUTLIM            *   FILE 070
//*             NON-STANDARD LABEL VERIFY ROUTINE                   *   FILE 070
//*             ALLOW GENERAL INQUIRY CMDS FROM RJP TERMS           *   FILE 070
//*             UPDATE GDG BASE LEVEL AT STEP END                   *   FILE 070
//*             JOB HEADER PAGE INFORMATION                         *   FILE 070
//*             ACCT (ACCT #) VALIDATION + DSP DICT.                *   FILE 070
//*             (PRE AJSW003) / RESTRICTED CLASS CHECKING           *   FILE 070
//*             DO NOT ALLOW PRTY=0 TO BE RELEASED                  *   FILE 070
//*             MAKE ANYLOCAL MEAN PRT3800 + PRT3211                *   FILE 070
//*             COMPUTE OSE PRIORITIES, CANCEL JUNK,                *   FILE 070
//*             MAKE SOME STARTED TASKS CLASS A                     *   FILE 070
//*             DEFINE USER FIELDS IN MACRO IATYTVT                 *   FILE 070
//*             COMPUTE JOB PRIORITY + CHANGE CLASS                 *   FILE 070
//*             JOB TRAILER PAGE INFORMATION                        *   FILE 070
//*             DON'T MLOG VERIFY MESSAGES DURING CONNECT           *   FILE 070
//*             ALLOW *T ALL COMMAND TO SEND TO ALL SYSTEMS         *   FILE 070
//*             ALLOW GENERIC STATUS AND CHECK OWNERSHIP            *   FILE 070
//*             SMF RECORDING FOR NJE SYSOUT DATASETS               *   FILE 070
//*             CHANGE MULTILEAVING DELAY TO .50 SECS               *   FILE 070
//*             RETURN NEW SECOND LEVEL MESSAGE TO STATUS           *   FILE 070
//*             PUT JULIAN DATE IN MLG MESSAGES(FROM EDSC)          *   FILE 070
//*             DELETE TIME STAMP FROM 3277 MESSAGES                *   FILE 070
//*             USE RQNETID IF NET = *NET-ID* FOR DJC WTO           *   FILE 070
//*             ALLOW ALL AS MPNAME ON *I G AND *F G CMDS           *   FILE 070
//*             BYPASS DESTINATION VALIDATION FOR XWTRS             *   FILE 070
//*             PUT DATASET LINECOUNT IN SSOB FOR XWTR              *   FILE 070
//*             ACF2 CODE FOR JCL PROCESSING                        *   FILE 070
//*             DON'T PRINT JESMSG, SYSMSG, JESJCL HEADERS          *   FILE 070
//*             DSP DICTIONARY ENTRIES                              *   FILE 070
//*             ADD INIT BLIP MESSAGE IAT0001                       *   FILE 070
//*             CREATE WRITE-TO-PROGRAMMER DSP (WTP)                *   FILE 070
//*             *V XXX,ALL WILL VARY DEVICE TO ALL SYSTEMS          *   FILE 070
//*             SYSLOG/EXTERNAL WTR EXECUTIVE                       *   FILE 070
//*             COST ESTIMATE INFO                                  *   FILE 070
//*             ENHANCEMENTS TO THE *I,B COMMAND                    *   FILE 070
//*             MODS TO JSM TO SCAN ALL JOBS + NO CANCEL            *   FILE 070
//*             PROGRAM TO ISSUE JES3 COMMANDS                      *   FILE 070
//*             JESOPER COMMAND                                     *   FILE 070
//*             ISSUE DEVICE CLOSE IF UNDER VM                      *   FILE 070
//*             SILO JES3 SUPPORT MODS                              *   FILE 070
//*             RESTRICTED CLASS VERIFICATON USERMOD                *   FILE 070
//*             VTAM USER EXIT (FRANK NASH)                         *   FILE 070
//*             3767 USER OUTPUT EXIT ROUTINE                       *   FILE 070
//*                                                                 *   FILE 070
~~~~~~~~~~~~~~~~

