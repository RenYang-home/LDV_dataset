# Large-scale Diverse Video (LDV) Dataset

The LDV 1.0 and LDV 2.0 datasets are established for Vidoe Enhancement Challenges in [NTIRE Workshop2021](https://data.vision.ee.ethz.ch/cvl/ntire21/) and [NTIRE Workshop2022](https://data.vision.ee.ethz.ch/cvl/ntire22/).

If the datasets and the benchmarks are useful for your research, please cite:
```
@inproceedings{yang2021dataset,
  title={{NTIRE 2021} Challenge on Quality Enhancement of Compressed Video: Dataset and Study},
  author={Ren Yang and Radu Timofte}, 
  booktitle={IEEE/CVF Conference on Computer Vision and Pattern Recognition Workshops}, 
  year={2021}
}

@inproceedings{yang2022ntire,
  title={{NTIRE 2022} Challenge on Super-Resolution and Quality Enhancement of Compressed Video: Dataset, Methods and Results},
  author={Ren Yang and Radu Timofte and others}, 
  booktitle={IEEE/CVF Conference on Computer Vision and Pattern Recognition Workshops}, 
  year={2022}
}
```

Should you have any questions, please feel free to contact:

Ren Yang @ ETH Zurich, Switzerland   

Email: ren.yang@vision.ee.ethz.ch


## LDV 1.0

The proposed LDV 1.0 in NTIRE 2021 contains 240 videos with diverse categories of content, different kinds of motion and various frame-rates. The dataset may be further extended in the future. The details of the proposed LDV 1.0 dataset are discribed in the dataset report:

> Ren Yang and Radu Timofte, "NTIRE 2021 Challenge on Quality Enhancement of Compressed Video: Dataset and Study", in IEEE/CVF Conference on Computer Vision and Pattern Recognition Workshops, 2021. [[Paper]](https://arxiv.org/abs/2104.10782)

### Download the LDV 1.0 dataset

- Training set (200 videos) 
[[Raw]](https://data.vision.ee.ethz.ch/reyang/training_raw.zip) 
[[Fixed QP]](https://data.vision.ee.ethz.ch/reyang/training_fixed-QP.zip)
[[Fixed bit-rate]](https://data.vision.ee.ethz.ch/reyang/training_fixed-rate.zip)
[[Info]](https://data.vision.ee.ethz.ch/reyang/data_train.xlsx)

- Validation set (20 videos)
[[Raw]](https://data.vision.ee.ethz.ch/reyang/validation_raw.zip)
[[Fixed QP]](https://data.vision.ee.ethz.ch/reyang/validation_fixed-QP.zip)
[[Fixed bit-rate]](https://data.vision.ee.ethz.ch/reyang/validation_fixed-rate.zip)
[[Info]](https://data.vision.ee.ethz.ch/reyang/data_validation.xlsx)

- Test set for Tracks 1 and 2 (10 videos)
[[Raw]](https://data.vision.ee.ethz.ch/reyang/test_raw_1.zip)
[[Fixed QP]](https://data.vision.ee.ethz.ch/reyang/test_fixed-QP_release.zip)
[[Fixed bit-rate]](https://data.vision.ee.ethz.ch/reyang/test_fixed-rate_1.zip)
[[Info]](https://data.vision.ee.ethz.ch/reyang/data_test_1.xlsx)

- Test set for Track 3 (10 videos)
[[Raw]](https://data.vision.ee.ethz.ch/reyang/test_raw_2.zip)
[[Fixed QP]](https://data.vision.ee.ethz.ch/reyang/test_fixed-QP_2.zip)
[[Fixed bit-rate]](https://data.vision.ee.ethz.ch/reyang/test_fixed-rate_release.zip)
[[Info]](https://data.vision.ee.ethz.ch/reyang/data_test_2.xlsx) 

The NTIRE 2021 challenge compresses videos in the **YUV domain** and evaluates results in the **RGB domain**. The following commands can be used to convert the videos to the YUV and RGB domains, respectively. 

```
ffmpeg -i xxx.mkv -pix_fmt yuv420p xxx.yuv
ffmpeg -i xxx.mkv ./xxx/%3d.png
```
