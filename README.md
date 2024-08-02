# MetalDiffusionMusicVis
An MLX based audio to visualization, via stable diffusion.

Idea is that I can take music signals(tempo,pitch) and then have them follow a a 2d trajectory which translates to the latent space being modified in the stable diffusion inference, generating music visualizations as parts of the image shift according to different signals shifting in the song. Hopefully, it can run in real time on consumer grade devices.

Learning Goals: diffusion noise methods, MLX, quantization, audio transforms

## TODO
- [X] Create circular UNet input noise walk
- [ ] Create circular clip latent walk
- [ ] Create segments in the image (inpainting), which each differ on their own walks
- [ ] Get signals from audio that can correspond with dominant melody, then get pitch into signal
- [ ] Real time performance (perhaps 1 step generation, or 1 step scheduler pass, or quantization, or mlx optimization... loading song first then playing it to simulate realtime)

## License

This project is licensed under the Non-Commercial License - see the [LICENSE](LICENSE) file for details.

Parts of this project incorporate code from [Original Repository]([https://github.com/username/repo](https://github.com/ml-explore/mlx-examples?tab=MIT-1-ov-file)) by [Original Author](https://github.com/ml-explore), which is licensed under the MIT License. See the [LICENSE-MIT](LICENSE-MIT) file for details.
