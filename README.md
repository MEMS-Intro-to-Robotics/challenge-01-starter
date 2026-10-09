# Challenge Homework 1: Design Your Own Arm: [Your Name]

ECE 383 / ME 555: Introduction to Robotics and Automation (Fall 2026)

Update this README with your name, NetID, and a 1–3 line summary of your work.

## Contents

- `display.launch.py`: shows your URDF in RViz with a slider for each joint.
  Run it from the repository root:
  `ros2 launch display.launch.py model:=<path to your .urdf.xacro>`
- `cad/`: your CAD files, or a text file with a link to them
- `docs/`: your three renderings and your RViz screenshot
- `test_challenge_1.py`: automated repository checks
- `pytest.ini`: limits `pytest` to `test_challenge_1.py` so it skips the ROS 2
  workspace

Create your description package under `ros2_ws/src/`. The help page for the
challenge homeworks has the package layout, mesh export guidance, and
troubleshooting notes:
https://mems-intro-to-robotics.github.io/guides/challenge_hw_help/

## Run the grading checks

From the repository root on the VM:

```bash
pytest -v
```

The checks confirm that the repository contains a description package with a
well-formed URDF or xacro file and mesh files, your CAD files or a link to them,
four readable images in `docs/`, and an updated README. They also flag tracked
ROS 2 build output.

The repository checks cover files and package setup. Course staff evaluate your
design, URDF, and design notes from your Gradescope PDF.

Before the final push, fix every failure and confirm that Classroom 50 reports a
passing result.
