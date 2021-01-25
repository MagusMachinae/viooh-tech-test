# VIOOH-tech-test

## Problem
Given a datasets of songs played, determine the top 10 songs played in the top 50 sessions
in the dataset, where a session is defined to be a collection of songs played by a given user where the interval between each element is not greater than 20 minutes.

## Usage

Clone the repo with ```git clone https://github.com/MagusMachinae/viooh-tech-test```
Due to storage limits on git-hub, it is necessary to download the data set from
http://ocelma.net/MusicRecommendationDataset/lastfm-1K.html
, placing it in ```resources/```, it is useful at this stage to rename the file containing the data of songs played to make the next step less tedious, the next step assumes it has been renamed to ```song-data.tsv```.
Call ```clojure (data->edn! "resources/song-data.tsv")``` to generate a set of files containing hash-maps of the data sorted by user.


## Notes and Commentary
While I had a strong intuition about how to go about solving the problem, but had difficulty concretely visualising each step, so I decided to start with focusing on IO and data parsing, which would also help me persist the results of each step and get data back that I could use to help reason about what data structures my functions need to operate on by generating output files.

Because of the nature of the problem, I decided to approach it more interactively, grabbing small sections of data to work on in the comment block, and gradually building up the logic and testing against generated data, naming processes once I had reached a clear boundary at which to mark progress.

## TODO



## License

Copyright © 2021 FIXME

This program and the accompanying materials are made available under the
terms of the Eclipse Public License 2.0 which is available at
http://www.eclipse.org/legal/epl-2.0.

This Source Code may also be made available under the following Secondary
Licenses when the conditions for such availability set forth in the Eclipse
Public License, v. 2.0 are satisfied: GNU General Public License as published by
the Free Software Foundation, either version 2 of the License, or (at your
option) any later version, with the GNU Classpath Exception which is available
at https://www.gnu.org/software/classpath/license.html.
