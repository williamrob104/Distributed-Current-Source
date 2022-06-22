# Distributed Current Source

## Introduction

Distributed current source (DCS) is a method for modeling the dynamic responses of eddy currents induced in objects. Both conductors and dielectrics as well as ferromagnetic and non-ferromagnetic materials are considered. Unlike conventional numerical methods such as finite element analysis, DCS accounts for eddy currents and magnetization by means of volume and surface current density sources, which gives closed-form solutions to eddy currents, magnetic flux density and electromotive force.

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
    <td>◯</td>
    <td>◯</td>
    <td>◯</td>
    <td>◯</td>
  </tr>
  <tr>
    <td>Ferromagnetic</td>
    <td>◯</td>
    <td>not FEA verified</td>
    <td>◯</td>
    <td>not FEA verified</td>
  </tr>
  <tr>
    <td>Ferroeletric</td>
    <td>◯</td>
    <td>not FEA verified</td>
    <td>not implemented</td>
    <td>not implemented</td>
  </tr>
</tbody>
</table>

### Features

- Multiple coils for excitation and sensing purposes
- Current or voltage excitation in both frequency and time domain

## Project Structure

The project is written in MATLAB, and verified using the COMSOL finite element analysis software. `.mlx` are matlab scripts and `.mph` are COMSOL files.

 `DCS_functions` directory contains the core functionalities and detailed formulation of DCS.

 `examples` directory contains examples of DCS applied to different problems as well as finite element analysis for comparison.
