BGEN files are pulled from https://bitbucket.org/gavinband/bgen/src/39c49c3c9029/example/?at=default

The Oxford-format BGEN and SAMPLE files are generated by QCTool V2, running the following command:

/gavinband-qctool-555945090429/build/release/qctool_v2.1-dev
    -g example.16bits.bgen
    -og example.16bits.oxford.bgen
    -bgen-omit-sample-identifier-block
    -os example.16bits.oxford.sample

The corrupted sample file is generated by taking the first four rows from the original sample file
and removing the trailing columns in the final row.

To generate comparison VCFs, the BGEN files are converted using QCTools:
https://bitbucket.org/gavinband/qctool