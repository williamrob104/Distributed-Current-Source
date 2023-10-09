# Distributed Current Source

## Introduction

Distributed current source (DCS) is a method for modeling the dynamic responses of eddy currents induced in objects. Material properties including electrical conductivity, permittivity, and magnetic permeability are considered. Unlike conventional numerical methods such as finite element method, DCS accounts for eddy currents and magnetization by means of volume and surface current sources, which gives closed-form solutions to eddy currents, magnetic flux density and electromotive force.

### Analysis types

<table class="tg">
<thead>
  <tr>
    <th rowspan="2"></th>
    <th colspan="2">Frequency domain</th>
    <th colspan="2">Time domain</th>
  </tr>
  <tr>
    <th>2D-axisymmetric</th>
    <th>3D</th>
    <th>2D-axisymmetric</th>
    <th>3D</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Non-ferromagnetic</td>
    <td>✅</td>
    <td>✅</td>
    <td>✅</td>
    <td>✅</td>
  </tr>
  <tr>
    <td>Ferromagnetic</td>
    <td>✅</td>
    <td>⚠️ not verified</td>
    <td>✅</td>
    <td>⚠️ not verified</td>
  </tr>
  <tr>
    <td>Ferroeletric</td>
    <td>✅</td>
    <td>✅</td>
    <td>❌</td>
    <td>❌</td>
  </tr>
</tbody>
</table>

### Features

- Multiple coils for excitation and sensing purposes
- Current or voltage excitation in both frequency and time domain
- Allow different conductivity for elements

## Project Structure

The project is written in MATLAB, and verified using the COMSOL finite element analysis software. `.mlx` are matlab scripts and `.mph` are COMSOL files.

 `DCS_functions` directory contains the core functionalities and detailed formulation of DCS.

 `examples` directory contains examples of DCS applied to different problems as well as finite element analysis for comparison.

 ## References

[1]	B. J. Hao, K. M. Lee, and K. Bai, "Distributed current source modeling method for 3D eddy current problem in magnetic conductor with discrete state-space J-phi formulation," J. Comput. Phys., vol. 401, Jan 15. 2020, doi: 10.1016/j.jcp.2019.109027.

