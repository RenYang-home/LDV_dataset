# Large-scale Diverse Video (LDV) Dataset

**Download the latest version: LDV 3.0 (365 videos)** [[Raw videos]](https://drive.google.com/file/d/1MT6oihhUuZDfaMSOZfH5SERxbUkHA4Je/view?usp=drive_link) [[Info]](https://drive.google.com/file/d/1_VTWRhrTKaNvMlR0UH-WZcWJibu1QwLt/view?usp=drive_link) 

The LDV 1.0, LDV 2.0 and LDV 3.0 datasets are established for the Video Enhancement Challenges in [NTIRE Workshop 2021](https://data.vision.ee.ethz.ch/cvl/ntire21/), [NTIRE Workshop 2022](https://data.vision.ee.ethz.ch/cvl/ntire22/) and [AIM Workshop 2022](https://data.vision.ee.ethz.ch/cvl/aim22/).

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

@inproceedings{yang2022aim,
  title={{AIM 2022} Challenge on Super-Resolution of Compressed Image and Video: Dataset, Methods and Results},
  author={Ren Yang and Radu Timofte and others}, 
  booktitle={European Conference on Computer Vision Workshops}, 
  year={2022}
}
```

Should you have any questions, please feel free to contact:

Ren Yang @ ETH Zurich, Switzerland   

Email: r.yangchn@gmail.com


## LDV 1.0 (240 videos)

The proposed LDV 1.0 in NTIRE 2021 contains 240 videos with diverse categories of content, different kinds of motion and various frame-rates. The dataset may be further extended in the future. The details of the proposed LDV 1.0 dataset are discribed in the dataset report:

> Ren Yang and Radu Timofte, "NTIRE 2021 Challenge on Quality Enhancement of Compressed Video: Dataset and Study", in IEEE/CVF Conference on Computer Vision and Pattern Recognition Workshops, 2021. [[Paper]](https://arxiv.org/abs/2104.10782)

### Download LDV 1.0

- Training set (200 videos) 
[[Raw]](https://drive.google.com/file/d/1E24fD2rGrB5QQWUl30RkczEkaGJlPBH_/view?usp=drive_link) 
[[Compressed (fixed QP)]](https://drive.google.com/file/d/1nhfzUHBUzQzhJO8GkpQtNW4vxu4tunNx/view?usp=drive_link)
[[Compressed (fixed bit-rate)]](https://drive.google.com/file/d/1SdIpIqeoQR-MgR0NS06eALL-I_vJjcIj/view?usp=drive_link)
[[Info]](https://drive.google.com/file/d/1SqRKyNxOE7cRb3TZ4JcPpe0r01zrpEq2/view?usp=drive_link)

- Validation set (20 videos)
[[Raw]](https://drive.google.com/file/d/19bNZhdjvRtbFCmOPzSJowCkjrk1dsecL/view?usp=drive_link)
[[Compressed (fixed QP)]](https://drive.google.com/file/d/1ANB85AI_2ShppyBkOEPvQKBHaS-HlPc1/view?usp=drive_link)
[[Compressed (fixed bit-rate)]](https://drive.google.com/file/d/1XLsytIMWjRYpkBD_CMiE5e9733dC4TvE/view?usp=drive_link)
[[Info]](https://drive.google.com/file/d/1wa4s7AOHpO2iWzK99sJbKaLna4pivmRM/view?usp=drive_link)

- Test set for Tracks 1 and 2 (10 videos)
[[Raw]](https://drive.google.com/file/d/1W4bDwhQbZpRyWmBlEAJZH6cte5-Blvn8/view?usp=drive_link)
[[Compressed (fixed QP)]](https://drive.google.com/file/d/1mc4LXrseNkpjLe9HfD0ho7g9JPHneKHy/view?usp=drive_link)
[[Compressed (fixed bit-rate)]](https://drive.google.com/file/d/1zeNSwd2D0D6vJ1hmXiOn0C2ug4IJmTca/view?usp=drive_link)
[[Info]](https://drive.google.com/file/d/1gS7Sis0tBvUA-xg96STEPaY2uTGYyGAM/view?usp=drive_link)

- Test set for Track 3 (10 videos)
[[Raw]](https://drive.google.com/file/d/1bCDGvmE_5ZQq7l4MRtJwyIMKWhj8JVxc/view?usp=drive_link)
[[Compressed (fixed QP)]](https://drive.google.com/file/d/1g08W8nIe6Hv8Mt7LZ0OoNNOPn478s_AR/view?usp=drive_link)
[[Compressed (fixed bit-rate)]](https://drive.google.com/file/d/1Y2pGoDN7yW7NeZ4bZy-UjmXUyaZwaJFd/view?usp=drive_link)
[[Info]](https://drive.google.com/file/d/18Hsm80F9h2_uEVoVoI4GNlZBvEAirYtw/view?usp=drive_link) 

The NTIRE 2021 challenge compresses videos in the **YUV domain** and evaluates results in the **RGB domain**. The following commands can be used to convert the videos to the YUV and RGB domains, respectively. 

```
ffmpeg -i xxx.mkv -pix_fmt yuv420p xxx.yuv
ffmpeg -i xxx.mkv ./xxx/%3d.png
```

## LDV 2.0 (LDV 1.0 + 95 videos = 335 videos)

The proposed LDV 2.0 in NTIRE 2022 contains 335 videos with diverse categories of content, different kinds of motion and various frame-rates. The details of the proposed LDV 2.0 dataset are discribed in the dataset report:

> Ren Yang, Radu Timofte, and others, "NTIRE 2022 Challenge on Super-Resolution and Quality Enhancement of Compressed Video: Dataset, Methods and Results", in IEEE/CVF Conference on Computer Vision and Pattern Recognition Workshops, 2022. [[Paper]](https://openaccess.thecvf.com/content/CVPR2022W/NTIRE/papers/Yang_NTIRE_2022_Challenge_on_Super-Resolution_and_Quality_Enhancement_of_Compressed_CVPRW_2022_paper.pdf)
> 

### Download LDV 2.0

- **The whole dataset (335 videos)** [[Raw videos]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/LDV2.zip) [[Info]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/data_LDV2.xlsx) 

- **Track 1**
  - Training set (LDV 1.0, 240 videos): 
[[Raw]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/train/train_gt.zip)
[[Compressed (Fixed QP)]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/train/train_QP37.zip)
[[Info]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/train/data_train_1.xlsx)
  - Validation set (15 videos): 
[[Raw]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/validation/track1_val_gt.zip)
[[Compressed (Fixed QP)]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/validation/validation_track1.zip)
[[Info]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/validation/data_val_1.xlsx)
  - Test set (15 videos): 
[[Raw]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/test/track1_test_gt.zip)
[[Compressed (Fixed QP)]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/test/test_track1.zip)
[[Info]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/test/data_test_1.xlsx)

- **Track 2** (The sizes of raw videos are cropped to the multiples of 16)
  - Training set (LDV 1.0, 240 videos): 
[[Raw]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/train/train_down2_gt.zip)
[[Compressed (Fixed QP)]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/train/train_down2_QP37.zip)
[[Info]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/train/data_train_2.xlsx)
  - Validation set (15 videos): 
[[Raw]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/validation/track2_val_gt.zip)
[[Compressed (Fixed QP)]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/validation/validation_track2.zip)
[[Info]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/validation/data_val_2.xlsx)
  - Test set (15 videos): 
[[Raw]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/test/track2_test_gt.zip)
[[Compressed (Fixed QP)]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/test/test_track2.zip)
[[Info]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/test/data_test_2.xlsx)

- **Track 3** (The sizes of raw videos are cropped to the multiples of 64)
  - Training set (LDV 1.0, 240 videos): 
[[Raw]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/train/train_down4_gt.zip)
[[Compressed (Fixed QP)]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/train/train_down4_QP37.zip)
[[Info]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/train/data_train_3.xlsx)
  - Validation set (15 videos): 
[[Raw]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/validation/track3_val_gt.zip)
[[Compressed (Fixed QP)]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/validation/validation_track3.zip)
[[Info]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/validation/data_val_3.xlsx)
  - Test set (15 videos): 
[[Raw]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/test/track3_test_gt.zip)
[[Compressed (Fixed QP)]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/test/test_track3.zip)
[[Info]](https://data.vision.ee.ethz.ch/reyang/NTIRE2022/test/data_test_3.xlsx)

The NTIRE 2022 challenge compresses videos in the **YUV domain** and evaluates results in the **RGB domain**. The following commands can be used to convert the videos to the YUV and RGB domains, respectively. 

```
ffmpeg -i xxx.mkv -pix_fmt yuv420p xxx.yuv
ffmpeg -i xxx.mkv ./xxx/%3d.png
```

## LDV 3.0 (LDV 2.0 + 30 videos = 365 videos)

The proposed LDV 3.0 in AIM 2022 contains 365 videos with diverse categories of content, different kinds of motion and various frame-rates. The details of the proposed LDV 3.0 dataset are discribed in the dataset report:

> Ren Yang, Radu Timofte, and others, "AIM 2022 Challenge on Super-Resolution of Compressed Image and Video: Dataset, Methods and Results", in European Conference on Computer Vision Workshops, 2022. [[Paper]](https://arxiv.org/pdf/2208.11184.pdf)
> 

### Download LDV 3.0

- **The whole dataset (365 videos)** [[Raw videos]](https://data.vision.ee.ethz.ch/reyang/AIM2022/LDV3.zip) [[Info]](https://data.vision.ee.ethz.ch/reyang/AIM2022/data_LDV3.xlsx) 

- **Track 2** (The sizes of raw videos are cropped to the multiples of 64)
  - Validation set (15 videos): 
[[Raw]](https://data.vision.ee.ethz.ch/reyang/AIM2022/video_val_gt.zip)
[[Compressed (Fixed QP)]](https://data.vision.ee.ethz.ch/reyang/AIM2022/video_val.zip)
[[Info]](https://data.vision.ee.ethz.ch/reyang/AIM2022/data_val_aim.xlsx)
  - Test set (15 videos): 
[[Raw]](https://data.vision.ee.ethz.ch/reyang/AIM2022/video_test_gt.zip)
[[Compressed (Fixed QP)]](https://data.vision.ee.ethz.ch/reyang/AIM2022/video_test.zip)
[[Info]](https://data.vision.ee.ethz.ch/reyang/AIM2022/data_test_aim.xlsx)

The AIM 2022 challenge compresses videos in the **YUV domain** and evaluates results in the **RGB domain**. The following commands can be used to convert the videos to the YUV and RGB domains, respectively. 

```
ffmpeg -i xxx.mkv -pix_fmt yuv420p xxx.yuv
ffmpeg -i xxx.mkv ./xxx/%3d.png
```
