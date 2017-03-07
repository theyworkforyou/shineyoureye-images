# Repository with images for the use of ShineYourEye

The images in this repository were generated with the
`multiple-thumbnail-sizes` branch of
[everypolitician/image_cache](https://github.com/everypolitician/image_cache/tree/multiple-thumbnail-sizes)
using a command like the following:

    EVERYPOLITICIAN_COUNTRY_SLUG=Nigeria \
        EXTRA_CSV='Governors:https://morph.io/everypolitician-scrapers/nigeria-state-governors/data.csv?key=MYMORPHKEY&query=select+%2A+from+%27data%27'
        \
        GITHUB_REPO=theyworkforyou/shineyoureye-images \
        GITHUB_ACCESS_TOKEN=MYPERSONALACCESSTOKEN \
        IMAGE_SIZES=original,250x250,100x100 \
        bundle exec bin/image_cache

You have to replace `MYMORPHKEY` and `MYPERSONALACCESSTOKEN` in
that command with an actual Morph API key and a
[GitHub personal access token](https://github.com/settings/tokens)
respectively.
