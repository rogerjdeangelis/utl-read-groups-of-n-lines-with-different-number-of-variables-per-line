# utl-read-groups-of-n-lines-with-different-number-of-variables-per-line
Read groups of n lines with different number of variables per line
    %let pgm=utl-read-groups-of-n-lines-with-different-number-of-variables-per-line;

    %stop_submission;

    Read groups of n lines with different number of variables per line

    github
    https://tinyurl.com/bp9ecj4a
    https://github.com/rogerjdeangelis/utl-read-groups-of-n-lines-with-different-number-of-variables-per-line

    sas communities
    https://tinyurl.com/mu9vz2rr
    https://communities.sas.com/t5/SAS-Programming/How-to-read-over-multiple-lines-record/m-p/807409#M318333

    Solution by
    ballardw
    https://communities.sas.com/t5/user/viewprofilepage/user-id/13884

    RELATED REPO

    https://github.com/rogerjdeangelis/utl-adding-infile-options-like-lrecl-and-recfm-to-cards-or-datalines-input
    https://github.com/rogerjdeangelis/utl-expanding-sas-string-functionality-by-loading-strings-into-the-infile-buffer
    https://github.com/rogerjdeangelis/utl-find-duplicate-values-in-different-columns-infile-processing
    https://github.com/rogerjdeangelis/utl-flag-non-missing-and-missing-words-with-one-or-zero-respectively-using-loadinfile-macro
    https://github.com/rogerjdeangelis/utl-fun-with-infile-processing-without-an-input-file-or-datalines
    https://github.com/rogerjdeangelis/utl-load-infile-with-a-string-and-parse-the-string-mutiple-arbitrary-length-delimeters
    https://github.com/rogerjdeangelis/utl-parsing-a-complex-string-using-input-infile-and-call-scan
    https://github.com/rogerjdeangelis/utl-pivot-text-file-wide-to-long-using-sas-infile-and-r
    https://github.com/rogerjdeangelis/utl-using-infile-and-input-to-split-strings
    https://github.com/rogerjdeangelis/utl-using-sas-infile-input-to-parse-compex-datastep-strings-empty-files
    https://github.com/rogerjdeangelis/utl-when-a-sentence-is-spread-over-many-lines-combine-lines-into-one-record-sas-infile-python



    /**************************************************************************************************************************/
    /*     INPUT            |      PROCESS               |                   OUTPUT                                           */
    /*                      |                            |                                                                    */
    /* REC1 11 12 13 14 15  | data want;                 | GRP  V1 V2 V3 V4 V5 V6 V7 V8 V9 V10 V11 V12                        */
    /* 16 17                |    infile cards n=4;       |                                                                    */
    /* 18 19                |    input                   | REC1 11 12 13 14 15 16 17 18 19  20  21  22                        */
    /* 20 21 22             |    #1 grp$ v1 v2 v3 v4 v5  | REC2 31 32 33 34 35 36 37 38 39  40  41  42                        */
    /* REC2 31 32 33 34 35  |    #2 v6 v7                |                                                                    */
    /* 36 37                |    #3 v8 v9                |                                                                    */
    /* 38 39                |    #4 v10 v11 v12;         |                                                                    */
    /* 40 41 42             | cards4;                    |                                                                    */
    /*                      | REC1 11 12 13 14 15        |                                                                    */
    /*                      | 16 17                      |                                                                    */
    /*                      | 18 19                      |                                                                    */
    /*                      | 20 21 22                   |                                                                    */
    /*                      | REC2 31 32 33 34 35        |                                                                    */
    /*                      | 36 37                      |                                                                    */
    /*                      | 38 39                      |                                                                    */
    /*                      | 40 41 42                   |                                                                    */
    /*                      | ;;;;                       |                                                                    */
    /*                      | run;quit;                  |                                                                    */
    /**************************************************************************************************************************/

    /*              _
      ___ _ __   __| |
     / _ \ `_ \ / _` |
    |  __/ | | | (_| |
     \___|_| |_|\__,_|

    */
