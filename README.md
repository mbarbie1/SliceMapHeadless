# SliceMap

Whole brain tissue slices are commonly used in neurobiological research for analyzing pathological features in an anatomically defined manner. However, since many pathologies are expressed in specific regions of the brain, it is necessary to have an annotation of the regions in the brain slices. Such an annotation can be done by manual delineation, as done most often, or by an automated region annotation tool. 

SliceMap is a FIJI/ImageJ plugin for automated brain region annotation of fluorescent brain slices. The plugin uses a reference library of pre-annotated brain slices (the brain region templates) to annotate brain regions of unknown samples. To perform the region annotation, SliceMap registers the reference slices to the sample slice (using elastic registration plugin BUnwarpJ) and uses the resulting image transformations to morph the template regions towards the anatomical brain regions of the sample. The resulting brain re-gions are saved as FIJI/ImageJ ROI’s (Regions Of Interest) as a single zip-file for each sample slice.

## Getting started

SliceMap is a FIJI (ImageJ) plugin. Fiji can be downloaded from www.fiji.sc.

The example dataset with 60 downscaled brain slices and brain region annotations can be found in the dataset subfolder

To install the SliceMap plugin, copy the jar-file SliceMap_-1.0-SNAPSHOT-jar-with-dependencies.jar into the plugins folder of the ImageJ/FIJI application (typically this folder is …/Fiji.app/plugins/). The plugin can then be called from Plugins > SliceMap > SliceMap. 

To use SliceMap directly one can also just start it (by e.g. double clicking it), this way it will open its own ImageJ instance to run in.

Further explaination of the usage and input/output of the SliceMap plugin is given in the *user_manual.pdf* file.

## Authors

Michael Barbier and Winnok De Vos

## License

This project is licensed under the MIT License - see the LICENSE.md file for details